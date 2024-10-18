# MiniMinter

MiniMinter is a web-based application that allows users to upload photos and create personalized NFT images based on elemental themes. Users can choose from various templates (Fire, Water, Earth, Air, and Space) and overlay their uploaded photos onto these templates to generate unique images. These images can then be optionally minted as NFTs and shared on social media.

## Table of Contents

- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Customization](#customization)
- [Technologies Used](#technologies-used)
- [License](#license)

## Features

- **Image Upload**: Users can upload a photo from their device to be used in creating the NFT.
- **Elemental Templates**: Users can choose from different elemental themes: Fire, Water, Earth, Air, and Space.
- **Canvas Drawing**: Uploaded photos are drawn over the chosen template using HTML Canvas.
- **Base64 Conversion**: After the image is created, it is converted to Base64 format for further use, such as minting or sharing.
- **NFT Minting**: Users can mint their customized image as an NFT (integration with an NFT minting service).
- **Email Submission**: Users provide their email address, which can be stored or used for further notifications.

## Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/your-username/MiniMinter.git
   cd MiniMinter
   ```

2. **Install dependencies**:
   ```bash
   npm install
   ```

3. **Run the development server**:
   ```bash
   npm run dev
   ```

   The application will start on `http://localhost:3000`.

## Usage

1. **Upload Photo**: Click the "Choose Photo" button to upload your image (supported formats: `.jpg`, `.jpeg`, `.png`).
2. **Select Theme**: Choose one of the elemental themes (Fire, Water, Earth, Air, or Space) from the dropdown menu.
3. **Submit**: Click "Submit" to generate the customized image. The image will be drawn over the selected template.
4. **Optional NFT Minting**: After the image is generated, you can mint it as an NFT and receive the NFT link for sharing.

## Customization

- **Change Templates**: To add new templates, place the images inside the `src/assets/` folder and update the theme selection logic in `PhotoUpload.jsx`.
- **Integrate with NFT Service**: To enable NFT minting, integrate with an NFT minting platform of your choice by modifying the backend logic to send the Base64 image data.
- **Change Styles**: You can customize the UI by editing `styles.css` to match your desired look and feel.

## Technologies Used

- **Frontend**: 
  - React.js
  - Vite (for fast development build)
  - MUI (Material UI) for styling
- **Image Handling**: 
  - HTML Canvas
  - FileReader API (to handle image uploads)
- **Optional**: 
  - Integration with third-party NFT minting platforms (e.g., OpenSea or other blockchain-based services)

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
