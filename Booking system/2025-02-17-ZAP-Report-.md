<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>ZAP by Checkmarx uusin</title>
<link
	href="2025-02-17-ZAP-Report-5/normalize/normalize.css" rel="stylesheet">
<link
	href="2025-02-17-ZAP-Report-5/themes/original/main.css" rel="stylesheet">
<link
	href="2025-02-17-ZAP-Report-5/themes/original/colors.css" rel="stylesheet">
</head>
<body>
	<header>
		<h1>ZAP by Checkmarx uusin</h1>
		<p>
			<span>Generated with</span> <a href="https://zaproxy.org"><img
				src="2025-02-17-ZAP-Report-5/zap32x32.png" alt="The ZAP logo" class="zap-logo">ZAP</a>
			<span>on Mon 17 Feb 2025, at 14:40:46</span>
		</p>
		<p>ZAP Version: 2.16.0</p>
		<p>
			ZAP by <a href="https://checkmarx.com/">Checkmarx</a>
		</p>
	</header>

	<main>

		<section id="contents" class="contents">
			<h2>Contents</h2>
			<nav>
				<ol>
					<li><a
						href="#about-this-report">About this report</a>
						<ol>
							
							<li><a
								href="#report-parameters">Report parameters</a></li>
						</ol></li>
					<data-th-block>
					<li><a
						href="#summaries">Summaries</a>
						<ol>
							<li><a
								href="#risk-confidence-counts">Alert counts by risk and confidence</a></li>
							<li><a
								href="#site-risk-counts">Alert counts by site and risk</a></li>
							<li><a
								href="#alert-type-counts">Alert counts by alert type</a></li>
						</ol></li>
					<li><a
						href="#alerts">Alerts</a>
						<ol>
							
							
							
							
							
							
							
							<li><a
								href="#alerts--risk-3-confidence-2"><span>Risk</span>=<span
									class="risk-level">High</span>, <span>Confidence</span>=<span
									class="confidence-level">Medium</span> <span>(1)</span></a></li>
							
							
							  
							 
							
							
							
							
							
							
							<li><a
								href="#alerts--risk-1-confidence-2"><span>Risk</span>=<span
									class="risk-level">Low</span>, <span>Confidence</span>=<span
									class="confidence-level">Medium</span> <span>(1)</span></a></li>
							
							
							  
							
							
							
							
							
							
							<li><a
								href="#alerts--risk-0-confidence-2"><span>Risk</span>=<span
									class="risk-level">Informational</span>, <span>Confidence</span>=<span
									class="confidence-level">Medium</span> <span>(1)</span></a></li>
							
							
							  
						</ol></li>
					<li><a
						href="#appendix">Appendix</a>
						<ol>
							<li><a
								href="#alert-types">Alert types</a></li>
						</ol></li>
					</data-th-block>
				</ol>
			</nav>
		</section>

		<section
			id="about-this-report" class="about-this-report">
			<h2>About this report</h2>

			

			<section
				id="report-parameters">
				<h3>Report parameters</h3>
				<div class="report-parameters--container">
					<h4>Contexts</h4>
					
					
					<p>No contexts were selected, so all contexts were included by default.</p>
					  

					<h4>Sites</h4>
					
					<p>The following sites were included:</p>
					<ul class="sites-list">
						<li><span class="site">http://localhost:8000</span></li>
					</ul>
					
					<p>(If no sites were selected, all sites were included by default.)</p>
					<p>An included site must also be within one of the included contexts for its data to be included in the report.</p>

					<h4>Risk levels</h4>
					<p>
						<span>Included</span>:
						 
						<span class="included-risk-codes"><span class="risk-level">High</span>, <span class="risk-level">Medium</span>, <span class="risk-level">Low</span>, <span class="risk-level">Informational</span></span>
					</p>
					<p>
						<span>Excluded</span>:
						 <span>None</span>
						
					</p>

					<h4>Confidence levels</h4>
					<p>
						<span>Included</span>:
						
						
						<span class="included-confidence-codes"><span class="confidence-level">User Confirmed</span>, <span class="confidence-level">High</span>, <span class="confidence-level">Medium</span>, <span class="confidence-level">Low</span></span>
					</p>
					<p>
						<span>Excluded</span>:
						
						
						<span class="included-confidence-codes"> <span class="confidence-level">User Confirmed</span>, <span class="confidence-level">High</span>, <span class="confidence-level">Medium</span>, <span class="confidence-level">Low</span>, <span class="confidence-level">False Positive</span></span>
					</p>
				</div>
			</section>
		</section>

		
		<section>
			
		</section>
		
		<section id="summaries" class="summaries">
			<h2>Summaries</h2>

			<section
				id="risk-confidence-counts">
				<h3>Alert counts by risk and confidence</h3>
				<table class="risk-confidence-counts-table">
					<caption>
						<p>This table shows the number of alerts for each level of risk and confidence included in the report.</p>
						<p>(The percentages in brackets represent the count as a percentage of the total number of alerts included in the report, rounded to one decimal place.)</p>
					</caption>
					<colgroup>
						<col>
						<col>
					</colgroup>
					<colgroup>
						<col
							style="width: 14.0%"><col
							style="width: 14.0%"><col
							style="width: 14.0%"><col
							style="width: 14.0%">
						<col style="width: 14.0%">
					</colgroup>
					<thead>
						<tr>
							<td colspan="2" rowspan="2"></td>
							<th scope="colgroup"
								colspan="5">Confidence</th>
						</tr>
						<tr>
							<th scope="col">User Confirmed</th>
							<th scope="col">High</th>
							<th scope="col">Medium</th>
							<th scope="col">Low</th>
							<th scope="col">Total</th>
						</tr>
					</thead>
					<tbody>
						<tr>
							<th scope="rowgroup"
								rowspan="5">Risk</th>
							<th scope="row">High</th>
							<td><span>0</span><br> <span
								class="additional-info-percentages">(0.0%)</span></td>
							<td><span>0</span><br> <span
								class="additional-info-percentages">(0.0%)</span></td>
							<td><span>1</span><br> <span
								class="additional-info-percentages">(33.3%)</span></td>
							<td><span>0</span><br> <span
								class="additional-info-percentages">(0.0%)</span></td>
							<td><span>1</span><br> <span class="additional-info-percentages">(33.3%)</span></td>
						</tr>
						<tr>
							
							<th scope="row">Medium</th>
							<td><span>0</span><br> <span
								class="additional-info-percentages">(0.0%)</span></td>
							<td><span>0</span><br> <span
								class="additional-info-percentages">(0.0%)</span></td>
							<td><span>0</span><br> <span
								class="additional-info-percentages">(0.0%)</span></td>
							<td><span>0</span><br> <span
								class="additional-info-percentages">(0.0%)</span></td>
							<td><span>0</span><br> <span class="additional-info-percentages">(0.0%)</span></td>
						</tr>
						<tr>
							
							<th scope="row">Low</th>
							<td><span>0</span><br> <span
								class="additional-info-percentages">(0.0%)</span></td>
							<td><span>0</span><br> <span
								class="additional-info-percentages">(0.0%)</span></td>
							<td><span>1</span><br> <span
								class="additional-info-percentages">(33.3%)</span></td>
							<td><span>0</span><br> <span
								class="additional-info-percentages">(0.0%)</span></td>
							<td><span>1</span><br> <span class="additional-info-percentages">(33.3%)</span></td>
						</tr>
						<tr>
							
							<th scope="row">Informational</th>
							<td><span>0</span><br> <span
								class="additional-info-percentages">(0.0%)</span></td>
							<td><span>0</span><br> <span
								class="additional-info-percentages">(0.0%)</span></td>
							<td><span>1</span><br> <span
								class="additional-info-percentages">(33.3%)</span></td>
							<td><span>0</span><br> <span
								class="additional-info-percentages">(0.0%)</span></td>
							<td><span>1</span><br> <span class="additional-info-percentages">(33.3%)</span></td>
						</tr>
						<tr>
							<th scope="row">Total</th>
							<td><span>0</span><br> <span
								class="additional-info-percentages">(0.0%)</span></td>
							<td><span>0</span><br> <span
								class="additional-info-percentages">(0.0%)</span></td>
							<td><span>3</span><br> <span
								class="additional-info-percentages">(100.0%)</span></td>
							<td><span>0</span><br> <span
								class="additional-info-percentages">(0.0%)</span></td>
							<td><span>3</span><br> <span
								class="additional-info-percentages">(100%)</span></td>
						</tr>
					</tbody>
				</table>
			</section>

			<section
				id="site-risk-counts">
				<h3>Alert counts by site and risk</h3>
				<table class="site-risk-counts-table">
					<caption>
						<p>This table shows, for each site for which one or more alerts were raised, the number of alerts raised at each risk level.</p>
						<p>Alerts with a confidence level of &quot;False Positive&quot; have been excluded from these counts.</p>
						<p>(The numbers in brackets are the number of alerts raised for the site at or above that risk level.)</p>
					</caption>
					<colgroup>
						<col>
						<col>
					</colgroup>
					<colgroup>
						<col
							style="width: 16.25%"><col
							style="width: 16.25%"><col
							style="width: 16.25%"><col
							style="width: 16.25%">
					</colgroup>
					<thead>
						<tr>
							<td colspan="2" rowspan="2"></td>
							<th scope="colgroup" colspan="4">Risk</th>
						</tr>
						<tr>
							<th scope="col">
								<span>High</span><br>  <span
									class="additional-info-percentages">(= High)</span>  
							</th>
							<th scope="col">
								<span>Medium</span><br>   <span
									class="additional-info-percentages">(&gt;= Medium)</span> 
							</th>
							<th scope="col">
								<span>Low</span><br>   <span
									class="additional-info-percentages">(&gt;= Low)</span> 
							</th>
							<th scope="col">
								<span>Informational</span><br>   <span
									class="additional-info-percentages">(&gt;= Informational)</span> 
							</th>
						</tr>
					</thead>
					<tbody>
						<tr>
							<th scope="rowgroup"
								rowspan="1">Site</th>
							<th scope="row">http://localhost:8000</th>
							
							<td><span>1</span><br> <span
								class="additional-info-percentages">(1)</span></td>
							<td><span>0</span><br> <span
								class="additional-info-percentages">(1)</span></td>
							<td><span>1</span><br> <span
								class="additional-info-percentages">(2)</span></td>
							<td><span>1</span><br> <span
								class="additional-info-percentages">(3)</span></td>
							
						</tr>
					</tbody>
				</table>
			</section>

			<section
				id="alert-type-counts">
				<h3>Alert counts by alert type</h3>
				<table class="alert-type-counts-table">
					<caption>
						<p>This table shows the number of alerts of each alert type, together with the alert type&#39;s risk level.</p>
						<p>(The percentages in brackets represent each count as a percentage, rounded to one decimal place, of the total number of alerts included in this report.)</p>
					</caption>
					<thead>
						<tr>
							<th scope="col">Alert type</th>
							<th scope="col">Risk</th>
							<th scope="col">Count</th>
						</tr>
					</thead>
					<tbody>
						<tr>
							<th scope="row"><a
								href="#alert-type-0">SQL Injection</a></th>
							<td class="risk-level">High</td>
							<td><span>3</span><br> <span
								class="additional-info-percentages">(100.0%)</span></td>
						</tr>
						<tr>
							<th scope="row"><a
								href="#alert-type-1">X-Content-Type-Options Header Missing</a></th>
							<td class="risk-level">Low</td>
							<td><span>1</span><br> <span
								class="additional-info-percentages">(33.3%)</span></td>
						</tr>
						<tr>
							<th scope="row"><a
								href="#alert-type-2">User Agent Fuzzer</a></th>
							<td class="risk-level">Informational</td>
							<td><span>12</span><br> <span
								class="additional-info-percentages">(400.0%)</span></td>
						</tr>
					</tbody>
					<tfoot>
						<tr>
							<th scope="row">Total</th>
							<td></td>
							<td>3</td>
						</tr>
					</tfoot>
				</table>
			</section>
		</section>

		<section id="alerts" class="alerts">
			<h2>Alerts</h2>
			<ol>
				
				 
				
				
				
				
				<li id="alerts--risk-3-confidence-2">
					<h3>
						<span>Risk</span>=<span
							class="risk-level">High</span>, <span>Confidence</span>=<span
							class="confidence-level">Medium</span> <span>(1)</span>
					</h3>
					<ol>
						
						<li class="alerts--site-li">
							<h4>
								<span class="site">http://localhost:8000</span> <span>(1)</span>
							</h4>
							<ol>
								
								<li>
									<h5>
										<a
											href="#alert-type-0">SQL Injection</a> <span>(1)</span>
									</h5>
									<ol>
										<li><details>
												<summary>
													<span class="request-method-n-url">POST http://localhost:8000/register</span>
												</summary>
												
<table class="alerts-table">
	<tr>
		<th scope="row">Alert tags</th>
		<td>
			<ul class="alert-tags-list">
				<li>
					 <span>POLICY_SEQUENCE = </span>
				</li>
				<li>
					<span><a href="https://owasp.org/Top10/A03_2021-Injection/">OWASP_2021_A03</a></span> 
				</li>
				<li>
					<span><a href="https://cwe.mitre.org/data/definitions/89.html">CWE-89</a></span> 
				</li>
				<li>
					<span><a href="https://owasp.org/www-project-web-security-testing-guide/v42/4-Web_Application_Security_Testing/07-Input_Validation_Testing/05-Testing_for_SQL_Injection">WSTG-v42-INPV-05</a></span> 
				</li>
				<li>
					 <span>POLICY_API = </span>
				</li>
				<li>
					 <span>POLICY_DEV_FULL = </span>
				</li>
				<li>
					 <span>POLICY_QA_STD = </span>
				</li>
				<li>
					 <span>POLICY_QA_FULL = </span>
				</li>
				<li>
					<span><a href="https://owasp.org/www-project-top-ten/2017/A1_2017-Injection.html">OWASP_2017_A01</a></span> 
				</li>
				<li>
					 <span>POLICY_DEV_CICD = </span>
				</li>
				<li>
					 <span>POLICY_DEV_STD = </span>
				</li>
			</ul>
		</td>
	</tr>
	<tr>
		<th scope="row">Alert description</th>
		<td> 
<p>SQL injection may be possible.</p>
 </td>
	</tr>
	<tr>
		<th scope="row">Other info</th>
		<td> 
<p>The page results were successfully manipulated using the boolean conditions [Matti AND 1=1 -- ] and [Matti AND 1=2 -- ]</p>

<p>The parameter value being modified was NOT stripped from the HTML output for the purposes of the comparison.</p>

<p>Data was returned for the original parameter.</p>

<p>The vulnerability was detected by successfully restricting the data originally returned, by manipulating the parameter.</p>
 </td>
	</tr>
	<tr>
		<th scope="row">Request</th>
		<td><details open="open">
				<summary>Request line and header section (831 bytes)</summary>
				
				<pre><code>POST http://localhost:8000/register HTTP/1.1
Accept: text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.7
Accept-Encoding: gzip, deflate, br, zstd
Accept-Language: en-US,en;q=0.9
Cache-Control: max-age=0
Connection: keep-alive
content-length: 90
Content-Type: application/x-www-form-urlencoded
host: localhost:8000
Origin: http://localhost:8000
Referer: http://localhost:8000/register
Sec-Fetch-Dest: document
Sec-Fetch-Mode: navigate
Sec-Fetch-Site: same-origin
Sec-Fetch-User: ?1
Upgrade-Insecure-Requests: 1
User-Agent: Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/130.0.0.0 Safari/537.36
sec-ch-ua: &quot;Not?A_Brand&quot;;v=&quot;99&quot;, &quot;Chromium&quot;;v=&quot;130&quot;
sec-ch-ua-mobile: ?0
sec-ch-ua-platform: &quot;Linux&quot;

</code></pre>
				
				
			</details> <details class="request-body" open="open">
				<summary>Request body (90 bytes)</summary>
				
				<pre><code>username=Matti+AND+1%3D1+--+&amp;password=Mennink%C3%A4inen&amp;birthdate=2025-02-04&amp;role=reserver</code></pre>
				
				
			</details></td>
	</tr>
	<tr>
		<th scope="row">Response</th>
		<td><details open="open">
				<summary>Status line and header section (159 bytes)</summary>
				
				<pre><code>HTTP/1.1 500 Internal Server Error
content-type: text/plain; charset=UTF-8
vary: Accept-Encoding
content-length: 25
date: Mon, 17 Feb 2025 12:38:03 GMT

</code></pre>
				
				
			</details> <details class="response-body" open="open">
				<summary>Response body (25 bytes)</summary>
				
				<pre><code>Error during registration</code></pre>
				
				
			</details></td>
	</tr>
	<tr>
		<th scope="row">Parameter</th>
		<td><pre><code>username</code></pre></td>
	</tr>
	<tr>
		<th scope="row">Attack</th>
		<td><pre><code>Matti AND 1=1 -- </code></pre></td>
	</tr>
	
	<tr>
		<th scope="row">Solution</th>
		<td> 
<p>Do not trust client side input, even if there is client side validation in place.</p>

<p>In general, type check all data on the server side.</p>

<p>If the application uses JDBC, use PreparedStatement or CallableStatement, with parameters passed by &#39;?&#39;</p>

<p>If the application uses ASP, use ADO Command Objects with strong type checking and parameterized queries.</p>

<p>If database Stored Procedures can be used, use them.</p>

<p>Do *not* concatenate strings into queries in the stored procedure, or use &#39;exec&#39;, &#39;exec immediate&#39;, or equivalent functionality!</p>

<p>Do not create dynamic SQL queries using simple string concatenation.</p>

<p>Escape all data received from the client.</p>

<p>Apply an &#39;allow list&#39; of allowed characters, or a &#39;deny list&#39; of disallowed characters in user input.</p>

<p>Apply the principle of least privilege by using the least privileged database user possible.</p>

<p>In particular, avoid using the &#39;sa&#39; or &#39;db-owner&#39; database users. This does not eliminate SQL injection, but minimizes its impact.</p>

<p>Grant the minimum database access that is necessary for the application.</p>
 </td>
	</tr>
</table>

											</details></li>
									</ol>
								</li>
								
							</ol>
						</li>
						
					</ol>
				</li>
				
				
				  
				 
				 
				
				
				
				
				<li id="alerts--risk-1-confidence-2">
					<h3>
						<span>Risk</span>=<span
							class="risk-level">Low</span>, <span>Confidence</span>=<span
							class="confidence-level">Medium</span> <span>(1)</span>
					</h3>
					<ol>
						
						<li class="alerts--site-li">
							<h4>
								<span class="site">http://localhost:8000</span> <span>(1)</span>
							</h4>
							<ol>
								
								<li>
									<h5>
										<a
											href="#alert-type-1">X-Content-Type-Options Header Missing</a> <span>(1)</span>
									</h5>
									<ol>
										<li><details>
												<summary>
													<span class="request-method-n-url">POST http://localhost:8000/register</span>
												</summary>
												
<table class="alerts-table">
	<tr>
		<th scope="row">Alert tags</th>
		<td>
			<ul class="alert-tags-list">
				<li>
					<span><a href="https://cwe.mitre.org/data/definitions/693.html">CWE-693</a></span> 
				</li>
				<li>
					<span><a href="https://owasp.org/Top10/A05_2021-Security_Misconfiguration/">OWASP_2021_A05</a></span> 
				</li>
				<li>
					<span><a href="https://owasp.org/www-project-top-ten/2017/A6_2017-Security_Misconfiguration.html">OWASP_2017_A06</a></span> 
				</li>
			</ul>
		</td>
	</tr>
	<tr>
		<th scope="row">Alert description</th>
		<td> 
<p>The Anti-MIME-Sniffing header X-Content-Type-Options was not set to &#39;nosniff&#39;. This allows older versions of Internet Explorer and Chrome to perform MIME-sniffing on the response body, potentially causing the response body to be interpreted and displayed as a content type other than the declared content type. Current (early 2014) and legacy versions of Firefox will use the declared content type (if one is set), rather than performing MIME-sniffing.</p>
 </td>
	</tr>
	<tr>
		<th scope="row">Other info</th>
		<td> 
<p>This issue still applies to error type pages (401, 403, 500, etc.) as those pages are often still affected by injection issues, in which case there is still concern for browsers sniffing pages away from their actual content type.</p>

<p>At &quot;High&quot; threshold this scan rule will not alert on client or server error responses.</p>
 </td>
	</tr>
	<tr>
		<th scope="row">Request</th>
		<td><details open="open">
				<summary>Request line and header section (831 bytes)</summary>
				
				<pre><code>POST http://localhost:8000/register HTTP/1.1
Accept: text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.7
Accept-Encoding: gzip, deflate, br, zstd
Accept-Language: en-US,en;q=0.9
Cache-Control: max-age=0
Connection: keep-alive
Content-Length: 76
Content-Type: application/x-www-form-urlencoded
Host: localhost:8000
Origin: http://localhost:8000
Referer: http://localhost:8000/register
Sec-Fetch-Dest: document
Sec-Fetch-Mode: navigate
Sec-Fetch-Site: same-origin
Sec-Fetch-User: ?1
Upgrade-Insecure-Requests: 1
User-Agent: Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/130.0.0.0 Safari/537.36
sec-ch-ua: &quot;Not?A_Brand&quot;;v=&quot;99&quot;, &quot;Chromium&quot;;v=&quot;130&quot;
sec-ch-ua-mobile: ?0
sec-ch-ua-platform: &quot;Linux&quot;

</code></pre>
				
				
			</details> <details class="request-body" open="open">
				<summary>Request body (76 bytes)</summary>
				
				<pre><code>username=Matti&amp;password=Mennink%C3%A4inen&amp;birthdate=2025-02-04&amp;role=reserver</code></pre>
				
				
			</details></td>
	</tr>
	<tr>
		<th scope="row">Response</th>
		<td><details open="open">
				<summary>Status line and header section (139 bytes)</summary>
				
				<pre><code>HTTP/1.1 200 OK
content-length: 29
content-type: text/plain;charset=UTF-8
date: Mon, 17 Feb 2025 12:34:45 GMT
vary: Accept-Encoding

</code></pre>
				
				
			</details> <details class="response-body" open="open">
				<summary>Response body (29 bytes)</summary>
				
				<pre><code>User registered successfully!</code></pre>
				
				
			</details></td>
	</tr>
	<tr>
		<th scope="row">Parameter</th>
		<td><pre><code>x-content-type-options</code></pre></td>
	</tr>
	
	
	<tr>
		<th scope="row">Solution</th>
		<td> 
<p>Ensure that the application/web server sets the Content-Type header appropriately, and that it sets the X-Content-Type-Options header to &#39;nosniff&#39; for all web pages.</p>

<p>If possible, ensure that the end user uses a standards-compliant and modern web browser that does not perform MIME-sniffing at all, or that can be directed by the web application/web server to not perform MIME-sniffing.</p>
 </td>
	</tr>
</table>

											</details></li>
									</ol>
								</li>
								
							</ol>
						</li>
						
					</ol>
				</li>
				
				
				  
				 
				
				
				
				
				<li id="alerts--risk-0-confidence-2">
					<h3>
						<span>Risk</span>=<span
							class="risk-level">Informational</span>, <span>Confidence</span>=<span
							class="confidence-level">Medium</span> <span>(1)</span>
					</h3>
					<ol>
						
						<li class="alerts--site-li">
							<h4>
								<span class="site">http://localhost:8000</span> <span>(1)</span>
							</h4>
							<ol>
								
								<li>
									<h5>
										<a
											href="#alert-type-2">User Agent Fuzzer</a> <span>(1)</span>
									</h5>
									<ol>
										<li><details>
												<summary>
													<span class="request-method-n-url">POST http://localhost:8000/register</span>
												</summary>
												
<table class="alerts-table">
	<tr>
		<th scope="row">Alert tags</th>
		<td>
			<ul class="alert-tags-list">
				
			</ul>
		</td>
	</tr>
	<tr>
		<th scope="row">Alert description</th>
		<td> 
<p>Check for differences in response based on fuzzed User Agent (eg. mobile sites, access as a Search Engine Crawler). Compares the response statuscode and the hashcode of the response body with the original response.</p>
 </td>
	</tr>
	
	<tr>
		<th scope="row">Request</th>
		<td><details open="open">
				<summary>Request line and header section (780 bytes)</summary>
				
				<pre><code>POST http://localhost:8000/register HTTP/1.1
Accept: text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.7
Accept-Encoding: gzip, deflate, br, zstd
Accept-Language: en-US,en;q=0.9
Cache-Control: max-age=0
Connection: keep-alive
Content-Length: 76
Content-Type: application/x-www-form-urlencoded
host: localhost:8000
Origin: http://localhost:8000
Referer: http://localhost:8000/register
Sec-Fetch-Dest: document
Sec-Fetch-Mode: navigate
Sec-Fetch-Site: same-origin
Sec-Fetch-User: ?1
Upgrade-Insecure-Requests: 1
user-agent: Mozilla/4.0 (compatible; MSIE 8.0; Windows NT 6.1)
sec-ch-ua: &quot;Not?A_Brand&quot;;v=&quot;99&quot;, &quot;Chromium&quot;;v=&quot;130&quot;
sec-ch-ua-mobile: ?0
sec-ch-ua-platform: &quot;Linux&quot;

</code></pre>
				
				
			</details> <details class="request-body" open="open">
				<summary>Request body (76 bytes)</summary>
				
				<pre><code>username=Matti&amp;password=Mennink%C3%A4inen&amp;birthdate=2025-02-04&amp;role=reserver</code></pre>
				
				
			</details></td>
	</tr>
	<tr>
		<th scope="row">Response</th>
		<td><details open="open">
				<summary>Status line and header section (159 bytes)</summary>
				
				<pre><code>HTTP/1.1 500 Internal Server Error
content-type: text/plain; charset=UTF-8
vary: Accept-Encoding
content-length: 25
date: Mon, 17 Feb 2025 12:37:11 GMT

</code></pre>
				
				
			</details> <details class="response-body" open="open">
				<summary>Response body (25 bytes)</summary>
				
				<pre><code>Error during registration</code></pre>
				
				
			</details></td>
	</tr>
	<tr>
		<th scope="row">Parameter</th>
		<td><pre><code>Header User-Agent</code></pre></td>
	</tr>
	<tr>
		<th scope="row">Attack</th>
		<td><pre><code>Mozilla/4.0 (compatible; MSIE 8.0; Windows NT 6.1)</code></pre></td>
	</tr>
	
	
</table>

											</details></li>
									</ol>
								</li>
								
							</ol>
						</li>
						
					</ol>
				</li>
				
				
				  
			</ol>
		</section>

		<section id="appendix" class="appendix">
			<h2>Appendix</h2>

			<section id="alert-types" class="alert-types">
				<h3>Alert types</h3>
				<p class="alert-types-intro">This section contains additional information on the types of alerts in the report.</p>
				<ol>
					<li
						id="alert-type-0">
						<h4>SQL Injection</h4>
						<table class="alert-types-table">
							<tr>
								<th scope="row">Source</th>
								<td>
									
									   <span>raised by an active scanner</span> <span>(<a
										href="https://www.zaproxy.org/docs/alerts/40018/">SQL Injection</a>)
									</span>   
								</td>
							</tr>
							<tr>
								<th scope="row">CWE ID</th>
								<td><a
									href="https://cwe.mitre.org/data/definitions/89.html">89</a></td>
							</tr>
							<tr>
								<th scope="row">WASC ID</th>
								<td>19</td>
							</tr>
							<tr>
								<th scope="row">Reference</th>
								<td>
									<ol>
										<li><a
											href="https://cheatsheetseries.owasp.org/cheatsheets/SQL_Injection_Prevention_Cheat_Sheet.html">https://cheatsheetseries.owasp.org/cheatsheets/SQL_Injection_Prevention_Cheat_Sheet.html</a></li>
									</ol>
								</td>
							</tr>
						</table>
					</li>
					<li
						id="alert-type-1">
						<h4>X-Content-Type-Options Header Missing</h4>
						<table class="alert-types-table">
							<tr>
								<th scope="row">Source</th>
								<td>
									
									   <span>raised by a passive scanner</span> <span>(<a
										href="https://www.zaproxy.org/docs/alerts/10021/">X-Content-Type-Options Header Missing</a>)
									</span>   
								</td>
							</tr>
							<tr>
								<th scope="row">CWE ID</th>
								<td><a
									href="https://cwe.mitre.org/data/definitions/693.html">693</a></td>
							</tr>
							<tr>
								<th scope="row">WASC ID</th>
								<td>15</td>
							</tr>
							<tr>
								<th scope="row">Reference</th>
								<td>
									<ol>
										<li><a
											href="https://learn.microsoft.com/en-us/previous-versions/windows/internet-explorer/ie-developer/compatibility/gg622941(v=vs.85)">https://learn.microsoft.com/en-us/previous-versions/windows/internet-explorer/ie-developer/compatibility/gg622941(v=vs.85)</a></li>
										<li><a
											href="https://owasp.org/www-community/Security_Headers">https://owasp.org/www-community/Security_Headers</a></li>
									</ol>
								</td>
							</tr>
						</table>
					</li>
					<li
						id="alert-type-2">
						<h4>User Agent Fuzzer</h4>
						<table class="alert-types-table">
							<tr>
								<th scope="row">Source</th>
								<td>
									
									   <span>raised by an active scanner</span> <span>(<a
										href="https://www.zaproxy.org/docs/alerts/10104/">User Agent Fuzzer</a>)
									</span>   
								</td>
							</tr>
							
							
							<tr>
								<th scope="row">Reference</th>
								<td>
									<ol>
										<li><a
											href="https://owasp.org/wstg">https://owasp.org/wstg</a></li>
									</ol>
								</td>
							</tr>
						</table>
					</li>
				</ol>
			</section>
		</section>
		 
	</main>
</body>
</html>



