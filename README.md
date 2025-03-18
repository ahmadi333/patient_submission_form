# Patient Submission Form

A custom WordPress solution designed to streamline patient data management through a submission form and advanced search functionality. This project leverages custom fields to store and query patient information efficiently.

## Features
- **Patient Submission Form**: Allows users to input patient details such as name, MRN, gender, contact, address, complaints, and surgical history.
- **Custom Field Search**: Enables searching patient records based on custom fields like `patient_details_name`, `patient_details_mrn`, etc., using a tailored WordPress query.
- **Shortcode Integration**: Includes a `[relevanssi_search]` shortcode for easy embedding of the search form in any page or post.
- **Responsive Design**: Built with flexibility in mind for seamless integration into WordPress themes.

## Installation
1. Clone or download this repository:  
   ```bash
   git clone https://github.com/ahmadi333/patient_submission_form.git
   ```
2. Copy the files into your WordPress theme's directory (e.g., `wp-content/themes/your-theme/`).
3. Add the code from `functions.php` to your theme’s `functions.php` file.
4. Create or edit `search.php` in your theme with the provided template to display search results.
5. Ensure the "patients" custom post type is registered in your WordPress setup (not included in this repo).

## Usage
- Use the shortcode `[relevanssi_search]` in any page or post to display the search form.
- Search by patient details (e.g., name, MRN, or address) to retrieve matching records.
- Customize the custom fields list in `functions.php` to match your specific patient data structure.

## Custom Fields
The search functionality targets the following custom fields:
- `patient_details_name`
- `patient_details_mrn`
- `patient_details_gender`
- `patient_details_contact`
- `patient_details_addresss`
- `presenting_complaints__complaint`
- `presenting_complaints__duration`
- `past_surgical_history_date_of_surgery`

## Requirements
- WordPress 5.0 or higher
- A theme with support for custom post types and templates

## Notes
- This project assumes a "patients" custom post type exists. You may need to register it separately if not already set up.
- For production use, ensure debugging is disabled in `wp-config.php` to avoid exposing errors.

## License
This project is open-source and available under the [MIT License](LICENSE).
