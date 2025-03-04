# BS_Project

This project demonstrates the creation of a responsive webpage using **HTML** and **Bootstrap**. The webpage consists of a navigation bar, a main content area, and a sign-in page. The layout dynamically adjusts based on the screen size.

## File Structure

![Project Structure](https://github.com/AniketP117/BootStrap_Project/blob/72bb8d2333b3979762d3ccae3e95a8993dbef574/Images/Screenshot%202025-03-04%20165057.png)

## Features
- Responsive **Navbar** with a Sign-In link
- **Landing Page** with a coffee theme and images
- **Sign-In Page** with a login form and a comment section
- Uses **Bootstrap 5.3.3** for styling and layout

## Files Included
- `BS.html` – Main landing page
- `signin.html` – Sign-in page with login form
- `README.md` – Project documentation
- `images/` – Folder containing images used in the project

## Technologies Used
- **HTML5**
- **Bootstrap 5.3.3** (CDN)

## How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/YOUR_USERNAME/BS_Project.git
   ```
2. Open `BS.html` or `signin.html` in your browser.

## Code Examples
### **Landing Page (`BS.html`)**
```html
<!DOCTYPE html>
<html lang="en">
<head>
  <title>Bootstrap Example</title>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet">
  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>
</head>
<body>
<nav class="navbar navbar-expand-sm navbar-dark bg-dark sticky-top">
  <div class="container-fluid">
    <a class="navbar-brand" href="#">Welcome</a>
    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#mynavbar">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="mynavbar">
      <ul class="navbar-nav me-auto">
        <li class="nav-item">
          <a class="nav-link" href="signin.html">Sign In</a>
        </li>
      </ul>
    </div>
  </div>
</nav>
</body>
</html>
```

### **Sign-In Page (`signin.html`)**
```html
<!DOCTYPE html>
<html lang="en">
<head>
  <title>Sign In</title>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet">
  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>
</head>
<body>
<div class="container p-5 my-5 bg-dark text-white" style="max-width: 600px;">
  <h1>Log In</h1>
  <form>
    <div class="mb-3">
      <label for="email" class="form-label">Email address</label>
      <input type="email" class="form-control" id="email" placeholder="Enter email">
    </div>
    <div class="mb-3">
      <label for="password" class="form-label">Password</label>
      <input type="password" class="form-control" id="password" placeholder="Enter password">
    </div>
    <button type="submit" class="btn btn-primary">Submit</button>
  </form>
</div>
</body>
</html>
```

## Images
Ensure that all images are placed in the `images/` directory and referenced correctly in the HTML files.

## Live Preview (Optional)
If hosted, you can provide a link here.

## License
This project is open-source and free to use.
