SERVER MANAGEMENT FOR INVENTORY SERVER

Directory creation and & organization:
.Create a directory named "inventory_server".
.Inside "inventory_server", create subdirectories for different product categories,
 such as "Electronics", "Furniture", "Clothing"
.Inside each category directory, organize product records by creating files named after individual products,
 including details like product IDs, names, and stock levels.

COMMAND:
	mkdir inventory_server
	cd inventory_server
	mkdir electronic furniture clothings
	touch electronics furniture clothings
	nano electronics furniture clothings
 
MOVE AND RENAME FILES:
.Move a file(products)from the "Electronics" category to the "Archived_Products" directory for discontinued items.
.rename a file within clothings dirctory


COMMAND:
	mv clothings clothings.txt
	mv ./electronics.txt ./archived_products


navigation & listing files:
.Navigate to the "inventory_server" directory and list its contents.
Verify the presence of all product category subdirectories and ensure
 that the inventory files for each product are correctly organized.


COMMAND:
	cd inventory_server
	ls -l


File permission management:
.Create a file named "inventory_report.csv" in the "inventory_server" directory, containing sensitive stock data
.Change the permissions of the file to restrict access,
 ensuring that only authorized staff members can view and modify the file.
Verify the changes by listing the file’s details and checking the permissions.

COMMAND:
	touch inventory_report.csv
	chmod 700 inventory_report.csv
 	ls -all

Backup files:
.Create a backup of important product data by copying them to a "backup" directory.
.Ensure that backups are regularly made to avoid data loss,
 especially for critical information like stock levels and sales data.



Removing files and directories:
.Delete obsolete inventory files, such as product records for
 discontinued items or outdated reports.
.Remove empty subdirectories from product categories that
 no longer contain inventory files or records.


Creating a script for file generation:
.Write a script that generates 100 dummy product files

COMMAND:
	touch inventory_report.csv
	nano inventory_report.csv

Exploring file history:
.View the command history to see the last 20 commands executed, particularly those related to 
file management in the "inventory_server" directory.

COMMAND:
	history 20

System Monitoring:
Check the server’s uptime to verify that the inventory management system is operating continuously.

COMMAND:
	uptime

Ping test and network verification:
.Perform a ping test to verify the server's network connectivity, ensuring that 
it can communicate with remote systems for inventory updates or data synchronization.
.Record the response times to ensure the network is
 performing optimally for data transfer and communication.

COMMAND:
	ping google.com

Search for Specific Files or Content:
.Use search commands to locate specific product files within the "inventory_server" directory.

COMMAND:
	grep -r inventory_server

Create a Directory for Each User:
.Set up individual directories for each inventory manager or
 team member to store data relevant to their area (e.g., product management,reporting, logistics).


COMMAND:
	mkdir manager
 	mkdir product management reporting logistics
	chmod 700 product management reporting logistics

File Sorting & Management:
.Sort the inventory files in the "Electronics" directory by file size to 
identify which product records are larger and may need more  storage or optimization.


COMMAND:
	 ls -l | sort -t. -k2

File Compression and Archive:
.Compress product data or inventory reports into a single archive file for long-term storage or transfer 
.Verify the contents of the archive to ensure all necessary files are included without extraction.

COMMAND:
	tar -czvf furniture.txt.gz furniture.txt
 
