#JobScrape

<h2> A Python API for scraping job listings from Indeed </h2>


<i>Please note that web scraping may be subject to the website's terms of service, so make sure to use this code responsibly and comply with any applicable legal requirements.</i>

It includes options to print results to the screen or save them in various file formats. The listings can be sorted by time/date posted, rank or rating, and salary/pay rate. Installation scripts for Windows, Mac, and Linux provided as well, setting up proper environmental variables, as well as installing required tools. 

You can execute the installation scripts on their respective platforms to set up the necessary environment and install the required packages. After that, you can run the Python API script to scrape Indeed job listings based on user input and save/print them in different formats.


Make sure to give the installation scripts executable permissions by running chmod +x *-install.sh


# Example usage:
job_name = input('Enter job name: ')
location = input('Enter location: ')
sort_by = input('Sort by (date/rank/salary): ')

job_listings = scrape_indeed_jobs(job_name, location, sort_by)

print_job_listings(job_listings)

# Save as JSON
save_job_listings(job_listings, 'job_listings.json', 'json')

# Save as CSV
save_job_listings(job_listings, 'job_listings.csv', 'csv')

# Save as DOCX
save_job_listings(job_listings, 'job_listings.docx', 'docx')

# Save as text
save_job_listings(job_listings, 'job_listings.txt', 'text')
      
