# Change Your Home IP
This Bash script configures /etc/hosts to:
Resolve localhost to 127.0.0.2.
Resolve facebook.com to 8.8.8.8.
## Implementation Notes:
Due to Docker’s restrictions on modifying /etc/hosts directly, the script:
Copies /etc/hosts to a temporary file.
Modifies the IP mappings with sed.
Replaces the original file with the modified version.

# Show Attached IPs
This Bash script displays all active IPv4 addresses on the machine.