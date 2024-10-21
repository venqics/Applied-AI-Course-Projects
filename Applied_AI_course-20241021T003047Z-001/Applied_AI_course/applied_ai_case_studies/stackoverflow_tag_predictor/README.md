# Problem Statement
Predict the tags (a.k.a. keywords, topics, summaries), given only the question text and its title.

# Business Objectives and Constraints
- Predict tags with high precision and recall
- No strict latency constraints.
- Machine Learning Problem
- Data
## Data contains 4 fields

- Id - Unique identifier for each question

- Title - The question’s title

- Body - The body of the question

- Tags - The tags associated with the question

**Number of rows in Train.csv** = 6034195


# Sample data point
- Id: 5
- Title: How to modify whois contact details?

Body:

```html <pre>
    <code>
    function modify(.......)
    {
        $mcontact = file_get_contents( "https://test.httpapi.com/api/contacts/modify.json?auth-userid=$uid&auth-password=$pass&contact-id=$cid&name=$name &company=$company&email=$email&address-line-1=$street&city=$city&country=$country&zipcode=$pincode&phone-cc=$countryCodeList[$phc]&phone=$phone" );
        $mdetails = json_decode( $mcontact, true );
        return $mdetails;
    }
    </code>
</pre>
<p>using this modify function, displays warning mesage</p>
<pre class="lang-none prettyprint-override">
    <code>
    Warning: file_get_contents(https://...@hihfg.com&address-line-1=3,dfgdf,fgdf&city=dfgfd&country=India&zipcode=641005&phone-cc=91&phone=756657)
        [function.file-get-contents]: failed to open stream: HTTP request failed!
        HTTP/1.0 400 Bad request in /home/gfdgfd/public_html/new_one/customer/account/class.whois.php on line 49\n
    </code>
</pre>
<p>Please help me, modify contact details.</p>```
