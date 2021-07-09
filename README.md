# WebAPIResponseCompression
<br>without compression file size in Chrome Network Tab is <b>16.2 Kb</b>
            <b><br>Response Headers</b>
            <br>Content-Type: text/plain; charset=utf-8
            <br>Date: Fri, 09 Jul 2021 00:09:23 GMT
            <br>Server: Kestrel
            <br>Transfer - Encoding: chunked

<br>with default compression (br) file size in Chrome Network Tab is <b>12.3 Kb</b>
            <br><b>Response Headers</b>
            <br>Content-Encoding: br
            <br>Content - Type: text / plain; charset = utf - 8
            <br>Date: Fri, 09 Jul 2021 00:14:22 GMT
            <br>Server: Kestrel
            <br>Transfer - Encoding: chunked
            <br>Vary: Accept - Encoding

<br>with br compression - optimal setting file size in Chrome Network Tab is <b>12.2 Kb</b> - best
            <br><b>Response Headers</b>
            <br>Content-Encoding: br
            <br>Content - Type: text / plain; charset = utf - 8
            <br>Date: Fri, 09 Jul 2021 00:14:22 GMT
            <br>Server: Kestrel
            <br>Transfer - Encoding: chunked
            <br>Vary: Accept - Encoding

            Response time is 14-21 ms for brotli

<br>with gzip compression -optimal setting-  file size in Chrome Network Tab is <b>12.3 Kb</b>
            <br><b>Response Headers</b>
            <br>Content-Encoding: gzip
            <br>Content - Type: text / plain; charset = utf - 8
            <br>Date: Fri, 09 Jul 2021 00:14:22 GMT
            <br>Server: Kestrel
            <br>Transfer - Encoding: chunked
            <br>Vary: Accept - Encoding

            Response time is 3-4 ms for gzip

<br>Gzip has the best response time , brotli has better compression ratio
