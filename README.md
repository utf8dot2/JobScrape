# JobScrape


<svg width="256" height="256" viewBox="0 0 256 256" fill="none" xmlns="http://www.w3.org/2000/svg">
  <style>
    @keyframes pulse {
      0% {
        transform: scale(1);
      }
      50% {
        transform: scale(1.2);
      }
      100% {
        transform: scale(1);
      }
    }
    rect, path {
      animation: pulse 2s infinite;
    }
  </style>
  <rect width="256" height="256" rx="60" fill="#0277BD" />
  <path d="M53.7527 102.651L56.6155 134.593H128.096V102.651H53.7527Z" fill="#EBEBEB" />
  <path d="M128.095 38H127.985H48L50.9036 69.9423H128.095V38Z" fill="#EBEBEB" />
  <path d="M128.095 218.841V185.608L127.955 185.645L92.3813 176.04L90.1072 150.564H72.821H58.0425L62.5175 200.718L127.948 218.882L128.095 218.841Z" fill="#EBEBEB" />
  <path d="M167.318 134.593L163.61 176.019L127.985 185.635V218.866L193.468 200.718L193.948 195.321L201.454 111.229L202.233 102.651L208 38H127.985V69.9423H172.994L170.088 102.651H127.985V134.593H167.318Z" fill="white" />
</svg>


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
      
