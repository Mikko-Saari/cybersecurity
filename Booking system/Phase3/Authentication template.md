# The Booking system - Phase 3



---

**2. Create a new page on Github (markdown) and add the following table to the page**

| **Page / Feature** | **Guest** | **Reserver** | **Administrator** |
|:----|:----:|:----:|:----:|
| `/` Resource                | | | |
| └─ View resource form      | ✅ | ✅ | ✅  |
| └─ Create new resource     | ✅  | ✅  | ✅  |
| `/`resources?id=1
| └─ View resource form      | ✅ can view the empty template | ✅ | ✅  |
| └─ modify resource         | ❌ | ✅  | ✅  |
| └─ delete resource         | ❌  | ❌  | ❌  |
| `/` reservation
| └─ View resource form      | ❌ | ✅ | ✅  |
| └─ Create new reservation  | ❌ | ✅ | ✅  |
| `/`reservation?id=2        
| └─ View resource form      | ❌ | ✅ | ✅  |
| └─ modify resource         | ❌ | ✅ | ✅  |
| `/`login       
| └─ View resource form      | ✅ | ✅ | ✅  |
| └─ modify resource         | ✅ | ✅ | ✅  |
| `/`logiout    
| └─ View resource form      | ✅ | ✅ | ✅  |
| └─ modify resource         | ✅ | ✅ | ✅  |




**Symbols used:**  
✅ Pass 
❌ Fail 
⚠️ Attention 






**5. Third testing technique: wfuzz and http**
- Try to find new pages using wfuzz and http commands.
- **Fill in the table as the testing progresses.**
- You can use, for example, the following commands:

**What kind of pages can be found using common words?**  
- **"login"**  
- **"logout"**  
- **"register"**  
- **"reservation"**  
- **"resources"**

```bash
wfuzz -c -w /usr/share/wordlists/dirb/common.txt --hc 404 http://localhost:8000/FUZZ
```

### Is There an API Folder and Pages Under It?  

Yes, an **API folder exists**, and the following pages were found under `/api/`:  

- **resources**  
- **session**  
- **users**  



```bash
wfuzz -c -w /usr/share/wordlists/dirb/common.txt --hc 404 http://localhost:8000/api/FUZZ
```

**Are there any pages in the reservations folder whose name is a number between 1-1000?**
```bash
wfuzz -c -z range,1-1000 --hc 404 http://localhost:8000/api/reservations/FUZZ
```
- Yes there is one.

**When the page is found, then what the page contains?**
```bash
http http://localhost:8000/api/reservations/1  
```
### Reservation Details  

The following data represents a reservation, including its start and end times, a unique reservation ID, and the associated resource.  

```json
{
    "reservation_id": 2,
    "reservation_start": "2025-03-12T15:23:00.000Z",
    "reservation_end": "2025-03-27T15:22:00.000Z",
    "reserver_token": "9a3d8817-bbcc-4dcc-914e-e3c795afdf80",
    "resource_id": 1
}

---

