
Static Website Hosting on Linux
Project Description
A complete demonstration of setting up and hosting a static website using Apache2 web server on Kali Linux. This project covers server installation, configuration, firewall setup, and custom website development.

Project Structure
text
static-website-linux/
│
├── index.html              # Main website file
├── README.md               # Project documentation
└── screenshots/            # Project screenshots
    ├── m1.png             # Apache installation
    ├── m2.png             # Firewall configuration
    ├── m3.png             # Service status
    ├── m4.png             # Default Apache page
    ├── m5.png             # Project directory creation
    ├── m6.png             # Website code editing
    ├── m7.png             # Final website preview
    └── m8.png             # Website content
Features
✅ Apache2 web server setup on Kali Linux

✅ UFW firewall configuration for web traffic

✅ Custom static website with modern design

✅ Responsive navigation and layout

✅ Professional CSS styling

✅ Service management with systemctl

Prerequisites
Kali Linux operating system

sudo privileges

Internet connection for package installation

Installation & Setup
1. Update System Packages
bash
sudo apt update
2. Install Apache2
bash
sudo apt install apache2 -y
3. Configure Firewall
bash
sudo ufw allow 'Apache'
4. Start and Enable Apache Service
bash
sudo systemctl start apache2
sudo systemctl enable apache2
5. Verify Service Status
bash
sudo systemctl status apache2
6. Create Project Directory
bash
mkdir my-website
cd my-website
7. Create Website Content
bash
nano index.html
8. Deploy Website
bash
sudo cp -r my-website/* /var/www/html/
sudo chown -R www-data:www-data /var/www/html/
sudo chmod -R 755 /var/www/html/
Website Features
Modern Design: Clean and professional interface

Responsive Layout: Adapts to different screen sizes

Navigation Bar: Easy site navigation

Hero Section: Eye-catching project introduction

Content Area: Detailed project information

Professional Styling: CSS-based visual enhancements

Technical Stack
Web Server: Apache2

Frontend: HTML5, CSS3

OS: Kali Linux

Tools: Terminal, Nano Editor, UFW Firewall

Accessing the Website
After deployment, access your website at:

text
http://localhost
or

text
http://your-server-ip
Project Screenshots
The project includes comprehensive documentation through screenshots showing each step of the implementation process.

Troubleshooting
Common Issues:
Apache not starting

bash
sudo systemctl restart apache2
sudo journalctl -u apache2
Permission issues

bash
sudo chown -R www-data:www-data /var/www/html/
sudo chmod -R 755 /var/www/html/
Firewall blocking access

bash
sudo ufw status
sudo ufw allow 'Apache'
Learning Outcomes
Linux server administration

Apache2 web server configuration

Firewall management with UFW

Static website development

Service management with systemctl

File permissions and ownership

Future Enhancements
Add SSL/TLS encryption

Implement virtual hosts

Add JavaScript functionality

Database integration

Deployment to cloud platform

Author
Your Name

Kali Linux Enthusiast

Web Development Learner

License
This project is open source and available under the MIT License.
