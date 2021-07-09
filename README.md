# WebAPIResponseCompression

without compression file size in Chrome Network Tab is 16.2 Kb
            // Response Headers
            // Content-Type: text/plain; charset=utf-8
            // Date: Fri, 09 Jul 2021 00:09:23 GMT
            // Server: Kestrel
            // Transfer - Encoding: chunked

with default compression (br) file size in Chrome Network Tab is 12.3 Kb
            // Response Headers
            // Content-Encoding: br
            // Content - Type: text / plain; charset = utf - 8
            // Date: Fri, 09 Jul 2021 00:14:22 GMT
            // Server: Kestrel
            // Transfer - Encoding: chunked
            // Vary: Accept - Encoding

with br compression - optimal setting file size in Chrome Network Tab is 12.2 Kb - best
            // Response Headers
            // Content-Encoding: br
            // Content - Type: text / plain; charset = utf - 8
            // Date: Fri, 09 Jul 2021 00:14:22 GMT
            // Server: Kestrel
            // Transfer - Encoding: chunked
            // Vary: Accept - Encoding

            // Response time is 14-21 ms for brotli

with gzip compression -optimal setting-  file size in Chrome Network Tab is 12.3 Kb
            // Response Headers
            // Content-Encoding: gzip
            // Content - Type: text / plain; charset = utf - 8
            // Date: Fri, 09 Jul 2021 00:14:22 GMT
            // Server: Kestrel
            // Transfer - Encoding: chunked
            // Vary: Accept - Encoding

            // Response time is 3-4 ms for gzip

Gzip has the best response time , brotli has better compression ratio
