# 📚 Library Management System

A role-based Library Management System built using React to manage library books, users, and borrowing activities through a clean, responsive, and user-friendly interface.

## 📌 Project Overview

The Library Management System is designed to simplify library operations by organizing books, managing users, and tracking book borrowing and returns.

The application supports four user roles: **Admin, Librarian, Staff, and Member**. Each role has specific permissions to ensure that users can access only the features relevant to them.

This project is being developed step by step to practice React concepts and build a practical frontend portfolio project.

## 🎯 Project Objectives

- Build a responsive and user-friendly web application.
- Practice React fundamentals through a real-world project.
- Implement role-based dashboards and permissions.
- Manage books and user information.
- Implement book issue and return workflows.
- Apply JavaScript array methods and business logic.
- Practice React Router, forms, validation, and state management.
- Maintain the project using Git and GitHub.
- Prepare for frontend developer interviews.

## 🛠️ Tech Stack

| Technology        | Purpose                                  |
| ----------------- | ---------------------------------------- |
| HTML5             | Application structure                    |
| CSS3              | Styling                                  |
| JavaScript (ES6+) | Application logic                        |
| React             | Component-based UI development           |
| Vite              | Development server and build tool        |
| Bootstrap         | Responsive layouts and UI styling        |
| Sass              | Organized and reusable styles            |
| React Router      | Navigation and routing                   |
| Git               | Version control                          |
| GitHub            | Source code hosting and project tracking |

Additional technologies, such as REST APIs and backend authentication, may be integrated in future stages.

## 👥 User Roles and Permissions

The application supports four roles with different access permissions.

### 1. Admin

- Add new books.
- Edit existing book details.
- View Librarian details.
- View Staff details.
- View Member details.
- Access administrative information.

### 2. Librarian

- Add new books.
- Edit existing book details.
- View Staff details.
- View Member details.
- Manage the book catalog.

### 3. Staff

- View available books.
- Borrow a maximum of **10 books at a time**.
- View their own borrowed books.
- View their own borrowing history.

### 4. Member

- View available books.
- Borrow a maximum of **3 books at a time**.
- View their own borrowed books.
- View their own borrowing history.

### Role Permission Matrix

| Feature                    | Admin         | Librarian     | Staff       | Member      |
| -------------------------- | ------------- | ------------- | ----------- | ----------- |
| Add books                  | ✅             | ✅             | ❌           | ❌           |
| Edit books                 | ✅             | ✅             | ❌           | ❌           |
| View Librarian details     | ✅             | ❌             | ❌           | ❌           |
| View Staff details         | ✅             | ✅             | Own profile | ❌           |
| View Member details        | ✅             | ✅             | ❌           | Own profile |
| Browse books               | ✅             | ✅             | ✅           | ✅           |
| Borrow books               | To be defined | To be defined | Up to 10    | Up to 3     |
| View own borrowing history | To be defined | To be defined | ✅           | ✅           |

**Note:** Borrowing limits for Admin and Librarian will be decided separately. The permission matrix will be enforced through application logic and, when a backend is integrated, server-side authorization.

## 🗺️ Development Roadmap

The project will be developed in eight phases. Each phase focuses on specific functionality and React concepts.

### Phase 1: Login

**Features**

- Create a login page with a clean UI.
- Add username and password fields.
- Implement controlled inputs.
- Validate form fields.
- Handle form submission.
- Prepare the login flow for the four user roles.

**React concepts**

- `useState`
- Controlled inputs
- Forms and event handling
- Conditional rendering
- Form validation

**Progress**

- [ ] Design the login page.
- [ ] Create reusable form components where appropriate.
- [ ] Implement input handling.
- [ ] Add validation messages.
- [ ] Test the login form.

### Phase 2: Routing and Layout

**Features**

- Configure application routes.
- Create a common Navbar and Sidebar.
- Build reusable page layouts.
- Prepare separate navigation for each role.

**React concepts**

- React Router
- Components and props
- Nested routes
- `Outlet`
- Layout components

**Progress**

- [ ] Install and configure React Router.
- [ ] Create the Navbar.
- [ ] Create the Sidebar.
- [ ] Create the common layout.
- [ ] Configure routes for the application.
- [ ] Prepare role-specific navigation.

### Phase 3: Dashboard

**Features**

- Create dashboards for Admin, Librarian, Staff, and Member.
- Display relevant statistics.
- Show book and borrowing summaries.
- Provide navigation to permitted features.

**React concepts**

- Components
- Props
- `map()`
- Reusable cards
- Conditional rendering

**Progress**

- [ ] Design the dashboard layout.
- [ ] Create reusable summary cards.
- [ ] Display dashboard statistics.
- [ ] Implement role-specific dashboard content.
- [ ] Test dashboard navigation.

### Phase 4: Book Management

**Features**

- Display the book catalog.
- Show book titles, authors, categories, and availability.
- Add new books.
- Edit existing book details.
- Delete books where permitted.
- Display book details.

**React concepts**

- CRUD operations
- Arrays and objects
- `map()`
- `filter()`
- `find()`
- State updates and immutability

**Progress**

- [ ] Create the book listing page.
- [ ] Display book information.
- [ ] Implement the Add Book form.
- [ ] Implement Edit Book functionality.
- [ ] Implement Delete Book functionality.
- [ ] Restrict book management actions to Admin and Librarian.
- [ ] Test book management operations.

### Phase 5: Members and Users

**Features**

- Manage member records.
- Display relevant user details.
- Create and edit user forms where permitted.
- Display role-specific profile information.
- Restrict access to user details according to permissions.

**React concepts**

- Forms
- Controlled inputs
- State management
- Conditional rendering
- JavaScript objects and arrays

**Progress**

- [ ] Create the user listing page.
- [ ] Create the user details view.
- [ ] Display relevant Staff and Member information.
- [ ] Implement permitted user management actions.
- [ ] Apply role-based access rules.
- [ ] Test user permissions.

### Phase 6: Issue and Return Books

**Features**

- Issue books to eligible users.
- Record borrowing and return information.
- Track borrowed books.
- Display due dates and return status.
- Enforce Staff and Member borrowing limits.
- Prevent borrowing unavailable books.

**Borrowing rules**

- Staff: Maximum 10 books at a time.
- Member: Maximum 3 books at a time.

**React concepts**

- Business logic
- Combining related data
- Updating arrays and objects
- State management
- Validation
- Conditional rendering

**Progress**

- [ ] Create the Issue Book interface.
- [ ] Create the Return Book interface.
- [ ] Track issued books.
- [ ] Update book availability after issue and return.
- [ ] Enforce borrowing limits.
- [ ] Prevent issuing unavailable books.
- [ ] Test issue and return scenarios.

### Phase 7: Search, Filters, and Reports

**Features**

- Search books by title or author.
- Filter books by category and availability.
- Sort book lists.
- View borrowing records.
- Display relevant reports and summaries.

**React concepts**

- `filter()`
- `find()`
- `sort()`
- Derived data
- Search state
- Conditional rendering

**Progress**

- [ ] Implement book search.
- [ ] Add category filters.
- [ ] Add availability filters.
- [ ] Implement sorting.
- [ ] Create borrowing summaries.
- [ ] Test search and filtering.

### Phase 8: Polish and Finalization

**Features**

- Improve responsive design.
- Add loading states.
- Add error messages and empty states.
- Improve accessibility.
- Handle invalid user actions.
- Review application performance.

**React concepts**

- Conditional rendering
- Error and loading state management
- Reusable UI components
- Responsive design
- Component optimization

**Progress**

- [ ] Test mobile, tablet, and desktop layouts.
- [ ] Add loading indicators where needed.
- [ ] Add empty-state messages.
- [ ] Add appropriate error handling.
- [ ] Review accessibility.
- [ ] Test the main user workflows.
- [ ] Update project documentation.

## 📂 Planned Project Structure

```text
library-management-system/
├── public/
├── src/
│   ├── assets/
│   ├── components/
│   │   ├── common/
│   │   ├── layout/
│   │   └── books/
│   ├── pages/
│   │   ├── Login/
│   │   ├── Dashboard/
│   │   ├── Books/
│   │   ├── Members/
│   │   └── IssueReturn/
│   ├── routes/
│   ├── context/
│   ├── hooks/
│   ├── services/
│   ├── App.jsx
│   ├── main.jsx
│   └── index.css
├── index.html
├── package.json
├── package-lock.json
└── README.md
```

The folder structure may evolve as the project grows.

## 🚀 Getting Started

### Prerequisites

- Node.js
- npm
- Git
- Visual Studio Code or another code editor

### Installation

1. Clone the repository:

   ```bash
   git clone YOUR_GITHUB_REPOSITORY_URL
   ```

2. Navigate to the project directory:

   ```bash
   cd library-management-system
   ```

3. Install dependencies:

   ```bash
   npm install
   ```

4. Start the development server:

   ```bash
   npm run dev
   ```

5. Open the local URL displayed in the terminal.

## 🧪 Testing and Validation

Each phase will be tested before being marked complete.

Testing will cover:

- Form validation.
- Role-based feature visibility and permissions.
- Book creation and editing.
- Borrowing limit enforcement.
- Book issue and return workflows.
- Search, filters, and sorting.
- Responsive layouts.
- Error and empty states.

## 🔮 Future Enhancements

- REST API integration.
- Backend authentication and authorization.
- Database integration for persistent records.
- Secure role-based access control.
- Borrowing history and reporting.
- Automated testing.
- Deployment to a hosting platform.

## 📈 Project Status

**Current status:** Planning and setup.

Development will begin with Phase 1: Login and proceed through the eight phases.

Progress checkboxes will be updated as features are implemented and tested.

## 👩‍💻 Purpose

This project is being developed as a practical learning and portfolio project to strengthen React, JavaScript, UI development, and frontend interview skills.

## 📄 License

This project is intended for learning and portfolio development.
