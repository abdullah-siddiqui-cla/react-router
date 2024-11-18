# 1. Basic Routing
## Goal: Create a React app with three pages: `Home`, `About`, and `Contact`.
## Steps:
- Install React Router using `npm install react-router-dom`.
- Create components for each page.
- Use `BrowserRouter`, `Routes`, and `Route` to set up navigation.
- Add `Link` components for navigating between pages.

# 2. Default Route
## Goal: Redirect users to the Home page when visiting the root (/).
## Steps:
- Define a route for `/`.
- Use `<Navigate to="/home" />` to redirect users.

# 3. 404 Not Found Page
## Goal: Display a custom "Not Found" page for unmatched routes.
## Steps:
- Create a `NotFound` component.
- Add a route with `path="*"` to display the `NotFound` page.

# 4. Dynamic Routes
## Goal: Create a user profile page with dynamic routing (e.g., /users/:id).
## Steps:
- Create a `UserProfile` component.
- Use the `useParams` hook to extract the `id` from the URL.
- Display the user's information dynamically.

# 5. Query Parameters
## Goal: Add filtering functionality to a product listing page using query parameters (e.g., /products?category=electronics).
## Steps:
- Use `useSearchParams` to read query parameters.
- Update the displayed products based on the category parameter.
- Create links to filter products dynamically.

# 6. Nested Routes
## Goal: Add nested routing for sections within the About page (e.g., `/about/team`, `/about/company`).
## Steps:
- Define child routes using Route inside a parent route.
- Use the Outlet component to render nested content.
- Create links for navigating between the nested sections.
- Hint: To defined nested routes,
```
<Route path="/about" element={<AboutPage />}>
  <Route path="team" element={<AboutTeam />} />
  <Route path="company" element={<AboutCompany />} />
</Route>
```

# 7. Programmatic Navigation
## Goal: Navigate programmatically after an event (e.g., button click).
## Steps:
- Use the `useNavigate` hook to navigate to a different route.
- Implement a button that redirects to another page upon a click.

# 8. Breadcrumb Navigation
## Goal: Add breadcrumbs to display the current navigation path.
## Steps:
- Use `useLocation` to get the current route.
- Split the route into parts and map them into breadcrumb links.
