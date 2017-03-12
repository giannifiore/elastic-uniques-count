# elastic-uniques-count
An experimental fallbacking algorithm: from linear unique elements count to sublinear Flajolet-Martin for IP tracking.

`MEMORY=50 STARTMODE=exact ITERATIONS=200000 IPS=1500 npm run test` to generate 1500 IPs distributed within 200k entries. Algorithm will start with trivial algorthm (save in dict to check for set membership) and fallback to Flajolet-Martin when it reaches full memory (50 bytes. Actually 48 as an IP takes 4 bytes). 

![A demo: execution compared with real results](output/flajomartin.JPG?raw=true "Demo")
