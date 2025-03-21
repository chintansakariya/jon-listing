# Job Listings Plugin

## Overview
This WordPress plugin adds a custom post type (CPT) called "Job Listings" that allows you to create and manage job postings. It includes custom meta fields for job details such as company name, job location, salary range, and application deadline.

## Features
- Custom Post Type: `job_listing`
- Meta fields for job details
- REST API support
- Admin panel meta box for job information
- Secure data handling

---

## Installation
1. **Download the Plugin:**
   - Save the PHP file as `job-listings.php` in a folder named `job-listings`.
   - Compress the folder into a `.zip` file if needed.

2. **Upload & Activate:**
   - Go to **WordPress Admin > Plugins > Add New**.
   - Click **Upload Plugin** and upload the `.zip` file.
   - Click **Activate**.

3. **Flush Permalinks:**
   - Navigate to **Settings > Permalinks**.
   - Click **Save Changes** (even if you don’t change anything).

---

## Usage
1. **Adding a Job Listing:**
   - Go to **WordPress Admin > Job Listings > Add New**.
   - Enter job title and details in the editor.
   - Fill in the meta fields:
     - Company Name
     - Job Location
     - Salary (Min & Max)
     - Application Deadline
   - Click **Publish**.

2. **Viewing Job Listings:**
   - Visit `/jobs/` on your website (e.g., `https://yourdomain.com/jobs/`).
   - Individual job listings will be available at `/jobs/{job-title}/`.

3. **Editing a Job Listing:**
   - Navigate to **Job Listings** in the admin panel.
   - Click on a job listing to edit.
   - Update details and click **Update**.

---

## REST API Integration
To fetch job listings via REST API:
```
GET https://yourdomain.com/wp-json/wp/v2/job_listing
```

To get a single job listing:
```
GET https://yourdomain.com/wp-json/wp/v2/job_listing/{id}
```

---

## Troubleshooting
- **Meta fields not showing?** Ensure you’ve activated the plugin and flushed permalinks.
- **404 errors on job pages?** Go to **Settings > Permalinks** and click **Save Changes**.
- **Plugin not activating?** Ensure the file is inside `wp-content/plugins/job-listings/`.

---

## Support
For support, visit [WordPress Support Forum](https://wordpress.org/support/forums/) or contact the developer.

---

## License
This plugin is released under the [GPL-2.0 License](https://www.gnu.org/licenses/gpl-2.0.html).

