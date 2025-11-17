# OPEN-SOURCE-EX-2
# AIM
To configure SELinux policies so that an Apache webserver running on a non-standard port (82) can properly serve existing HTML content from /var/www/html, ensuring the website becomes accessible without altering or removing any files.

# PROCEDURE
1. Check the SELinux status

Verify whether SELinux is running in enforcing mode on the system.

2. Ensure the Apache webserver is running

Confirm that the webserver service is installed, enabled, and active.

3. Allow network access through the firewall

Make sure the system firewall allows traffic on the non-standard port (82).

4. Configure Apache to listen on port 82

Open the webserver configuration file and set the listening port to 82.

5. Verify that the HTML files exist

Check the /var/www/html directory to ensure all required HTML files are present.

6. Review existing SELinux port contexts

Check which ports are currently allowed for Apache under the SELinux policy.

7. Add port 82 to SELinux allowed ports

Update SELinux configuration so that Apache is permitted to use the non-standard port (82).

8. Confirm the SELinux port change

Recheck SELinux settings to ensure port 82 has been mapped to the appropriate webserver port type.

9. Validate SELinux file contexts

Ensure that the files under /var/www/html have the correct SELinux context for web content, and restore it if necessary.

10. Restart the webserver and test accessibility

Restart the Apache service and verify that the website loads correctly in a browser using port 82.

# Output
<img width="1145" height="848" alt="Screenshot 2025-09-22 091123" src="https://github.com/user-attachments/assets/ae7a6c0f-a4b1-4bfb-a9fa-bba382b41dec" />
<img width="1268" height="890" alt="Screenshot 2025-09-22 161006" src="https://github.com/user-attachments/assets/6882e153-5b72-48f2-b848-1bbe912def53" />
<img width="1153" height="864" alt="Screenshot 2025-09-22 161108" src="https://github.com/user-attachments/assets/1b987265-78c4-4a61-8de1-e56513083dab" />
<img width="761" height="550" alt="Screenshot 2025-09-22 161124" src="https://github.com/user-attachments/assets/889c08e8-2265-416a-bd8e-5acf43a4940b" />
<img width="1026" height="829" alt="Screenshot 2025-09-22 163557" src="https://github.com/user-attachments/assets/e3f063f1-c212-4d64-9d7d-379b835c7781" />
<img width="1062" height="353" alt="Screenshot 2025-09-22 163824" src="https://github.com/user-attachments/assets/78524493-bf9c-4aed-87bd-97be742d26ca" />
<img width="734" height="508" alt="Screenshot 2025-09-23 102306" src="https://github.com/user-attachments/assets/cc5d1cb8-edb0-494f-b5dd-7d53ff7f9e60" />
<img width="1146" height="488" alt="Screenshot 2025-09-23 102738" src="https://github.com/user-attachments/assets/72ef903a-eb1a-47c5-949b-dbc0c01ab147" />
<img width="722" height="526" alt="Screenshot 2025-09-23 112604" src="https://github.com/user-attachments/assets/a62e3130-bbf3-45bb-bb06-6faaeee6b58f" />


# RESULT
The SELinux configuration was successfully updated, enabling the Apache webserver to serve existing HTML content from /var/www/html on the non-standard port 82. The website became fully accessible without modifying any of the original files.
