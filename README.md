# Get-Azure-IP-Ranges.sh
Little bash script for automatically fetching the most recent Azure IP Ranges.
Great for automating things...

# Usage
```
$ ./get-ip-ranges
```
Will output the current Azure IP ranges to stdout
```
$ ./get-ip-ranges > az-ip-ranges.xml
```
Lets you redirect output to a file.
```
$ ./get-ip-ranges | vi -
```
Lets VIM read current Azure IP ranges from stdin.
```
$ ./get-ip-ranges | xmlstarlet sel -t -v "//@Subnet"
```
Outputs just the Azure IP range using xmlstarlet.
