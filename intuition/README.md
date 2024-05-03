# HTB: Intuition - Linux - Hard

* **[Machine Profile](https://app.hackthebox.com/machines/Intuition)**
* **Date Started:** 2024-05-03


## Discovery

Initial nmap scan revealed vhost: `comprezzor.htb`. Added to hosts file: `echo "10.129.151.184 comprezzor.htb" | sudo tee --append /etc/hosts`.

Navigated to site in browser. Site is a _file compression service_. 

  * Bottom of page has _Report_ link to report bugs. Added `report.comprezzor.htb` to hosts file to enable browsing to this subdomain. Clicking the _Report_ button to submit a bug redirects to another subdomain, `auth.comprezzor.htb`. Added this to hosts file as well.
  * Created an account on the `auth.comprezzor.htb` page to enable sign-on.
