# Vite + React + TypeScript Starter

This project is built using **Vite**, **React**, and **TypeScript** to provide a fast and efficient development environment.

## **Deplyment Link** 
Website : https://entnt-project-ten.vercel.app/


## **Getting Started**

### **Installation**

1. Clone the repository:
   ```bash
   git clone <your-repo-url>
   cd <repo-name>
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

### **Development Server**

To start the development server, run:
```bash
npm run dev
```
Visit [http://localhost:5173](http://localhost:5173) to view the application in the browser.

### **Production Build**

To build the application for production:
```bash
npm run build
```
The production-ready files will be in the `dist` directory.

### **Preview Build**

To locally preview the production build:
```bash
npm run preview
```

## **Deployment**

This application is ready to deploy on **Vercel**. Follow these steps:

1. Push the project to a GitHub repository.
2. Go to the [Vercel Dashboard](https://vercel.com/).
3. Import the GitHub repository and configure the build settings:
   - **Build Command**: `npm run build`
   - **Output Directory**: `dist`
4. Click **Deploy**. Vercel will provide a live URL for your app.

## **Application Functionality**

### **Admin Module**
- Allows admins to set up companies.
- Admins can configure communication parameters such as frequency and method.
- Tools for managing data related to companies and communication tasks.

### **User Module**
- Users can visualize, manage, and log communication tasks.
- Two views:
  - **Past Communications**: Displays all completed communications sorted by date.
  - **Upcoming Communications**: Lists all planned communications that are scheduled for future dates.

### **Notification System**
- Overdue communications are flagged.
- Communications due today are highlighted.
- Users can log communication events through a dedicated form.

### **Communication Logging**
- Supports logging communication for single or multiple companies at once.
- Fields include date, method, and optional notes.
- Automatically associates logged communications with the selected companies.

### **Dark Mode Support**
- Enhanced user interface for dark mode compatibility.
- Ensures proper contrast and visibility of all form elements.

### **Dynamic Filtering and Sorting**
- Filters communications based on time (past vs. upcoming).
- Sorts communications in descending order for past and ascending for upcoming tasks.

## **Known Limitations**

1. **Notification Accuracy**
   - The notification system relies on computed properties from data. If there are data inaccuracies (e.g., missing periodicity or incorrect communication logs), the notifications might not reflect the correct status.

2. **Limited Admin/User Separation**
   - Current implementation does not differentiate between admin and user modes at the authentication level. Both admin and user functionalities are accessible within the same UI, separated by tabs or sections. Future implementations might require proper role-based access control.

3. **Limited Data Validation**
   - Dependencies between communication methods, companies, and communications are not strictly enforced. Deleting a company or communication method could leave orphaned records.

---


