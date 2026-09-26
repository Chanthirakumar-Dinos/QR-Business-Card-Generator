# QR Business Card Generator

A modern, premium **QR Business Card Generator** that allows users to create a digital contact QR code and a downloadable business card from personal and professional information.

The application runs entirely in the browser and does not require a backend or database.

## ✨ Features

* Generate a personal contact QR code
* Generate a premium business card
* Download QR code as PNG
* Download business card as transparent PNG
* Upload company logo
* Drag & drop logo upload
* Logo preview and remove option
* Ignore logo option
* Multiple premium business card themes
* Light mode and dark mode
* Mobile responsive design
* Country-code selector for mobile numbers
* Mobile number validation
* Professional job-position selection
* Automatically creates a vCard QR code
* Optional email, company, job position, website, and address
* High-quality business card export using `html2canvas`

## 🎨 Business Card Themes

The application provides four premium themes:

1. **Ledger**

   * Dark green
   * Gold accents
   * Premium professional appearance

2. **Studio Mono**

   * Black and white
   * Minimal design
   * Modern appearance

3. **Coral Split**

   * Cream and coral
   * Split-color layout
   * Elegant business style

4. **Gold Seal**

   * Deep plum
   * Gold accents
   * Luxury appearance

## 📝 Personal Details

The following personal information can be entered:

* First Name
* Last Name
* Mobile Number
* Country Code
* Email Address

First name, last name, and mobile number are required fields.

## 💼 Professional Details

The application supports:

* Company name
* Job position
* Website
* Address
* Company logo

The job position field includes predefined positions and also allows users to enter a custom position.

## 🖼️ Company Logo

Users can upload a company logo in:

* PNG
* JPG
* SVG

The logo can be uploaded by:

* Clicking the upload area
* Dragging and dropping an image

Users can also remove the uploaded logo or enable **Ignore Logo**, which displays a brand dot instead.

## 📱 QR Code

The application generates a QR code containing the user's contact information in **vCard 3.0** format.

The QR code can contain:

* Name
* Mobile number
* Email
* Company
* Job position
* Website
* Address

The generated QR code uses high error correction for reliable scanning.

## 📥 Download Options

### QR Code

The generated QR code can be downloaded as:

```text
QR.png
```

### Business Card

The generated business card can be downloaded as:

```text
Business_Card.png
```

The business card is rendered at high quality using a scale factor of 4 and exported as a PNG with transparency.

## 🛠️ Technologies Used

### Frontend

* HTML5
* CSS3
* JavaScript
* Bootstrap 5.3.3

### Libraries

* **Bootstrap 5.3.3** – UI layout and responsive design
* **Font Awesome 6.5.2** – Icons
* **QRCode.js 1.0.0** – QR code generation
* **html2canvas 1.4.1** – Business card image export
* **Google Fonts**

  * Manrope
  * Fraunces
  * IBM Plex Mono

The external libraries are loaded through CDN links in the HTML file.

## 📂 Project Structure

```text
QR-Business-Card-Generator/
│
├── index.html
└── README.md
```

The current project can operate as a single HTML file because the HTML, CSS, and JavaScript are contained in the same document.

## 🚀 How to Run

### Method 1 – Open Directly

1. Download or copy the project.
2. Open `index.html`.
3. The application will open in your web browser.
4. Enter your contact details.
5. Select a business card theme.
6. Click **Generate Premium Card**.

No server is required for the basic application.

### Method 2 – VS Code

1. Open the project folder in Visual Studio Code.
2. Open `index.html`.
3. Install the **Live Server** extension if required.
4. Right-click `index.html`.
5. Select **Open with Live Server**.
6. The application will open in your browser.

## 📖 How to Use

### Step 1 – Enter Personal Details

Enter:

* First name
* Last name
* Country code
* Mobile number
* Email address

The application validates the mobile number before generating the card.

### Step 2 – Enter Professional Details

Add:

* Company
* Job position
* Website
* Address

All professional details except the company name are optional.

### Step 3 – Upload Company Logo

Click the logo upload area or drag and drop your logo.

If you do not want to use a logo, enable:

```text
Ignore logo (show brand dot instead)
```

### Step 4 – Select a Theme

Choose one of the available themes:

```text
Ledger
Studio Mono
Coral Split
Gold Seal
```

The selected theme is applied to the business card preview.

### Step 5 – Generate

Click:

```text
Generate premium card
```

The application generates both:

* Contact QR code
* Premium business card

### Step 6 – Download

Use:

```text
Download QR
```

to download the QR code.

Switch to the **Business Card** tab and use:

```text
Download Business Card
```

to export the business card.

## 🔐 Data & Privacy

This application is designed as a client-side browser application.

The entered contact information is processed by JavaScript in the browser to generate the vCard and QR code. The uploaded logo is also read locally using the browser's `FileReader` API.

There is no backend, database, login system, or server-side storage implemented in the provided HTML file.

> **Note:** External CDN resources are loaded from third-party services such as jsDelivr, Cloudflare, and Google Fonts.

## 📐 Responsive Design

The application includes responsive CSS for smaller devices.

On mobile screens:

* Form spacing is reduced
* Business card preview is scaled
* Card details change to a single-column layout
* Action buttons become full width
* Theme options adapt to smaller screens

## ⚙️ Validation

The mobile number validation checks that:

* A number is entered
* A country code is selected separately
* The user does not enter another `+` country code in the mobile field
* At least 6 digits are entered

## 🔄 Reset / Create New Card

The **Reset** button clears the current form.

The **Create New** button also clears the form, uploaded logo, QR code, and generated business card view so a new card can be created.

## 🧩 Main JavaScript Functions

Important functions included in the application:

| Function           | Purpose                             |
| ------------------ | ----------------------------------- |
| `handleLogoFile()` | Processes uploaded logo             |
| `clearLogo()`      | Removes uploaded logo               |
| `setTheme()`       | Changes business card theme         |
| `vcard()`          | Creates vCard contact information   |
| `generateQR()`     | Generates QR code                   |
| `validateMobile()` | Validates mobile number             |
| `showStatus()`     | Displays success/error messages     |
| `toggleField()`    | Shows or hides optional card fields |

## 🎯 Project Purpose

The purpose of this project is to provide a simple and attractive way for users to create a digital contact card containing a QR code.

Instead of manually sharing multiple contact details, users can provide a single QR code that can be scanned by another person to save the contact information.

## 🔮 Possible Future Improvements

The following features could be added in future versions:

* PDF business card export
* JPG export option
* Multiple business card sizes
* Custom logo size controls
* Custom QR code colors
* Custom fonts
* Custom background colors
* Social media links
* WhatsApp contact link
* LinkedIn profile
* Multiple QR code styles
* Save card designs
* Local storage support
* Print business card option
* Front and back business card designs
* Share card directly to social media
* PWA/mobile app support

## 📄 License

This project can be used and modified for educational and personal projects.

If third-party libraries are used, their respective licenses and terms should be followed.

## 👨‍💻 Project

**Project Name:** QR Business Card Generator

**Type:** Frontend Web Application

**Technology:** HTML, CSS & JavaScript

**Output:** QR Code + Premium Business Card

**Responsive:** Yes

**Backend Required:** No
