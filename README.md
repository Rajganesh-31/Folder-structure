# Folder structure
## Frontend
```
/src
│
├── pages/                            ← Route-based pages
│   ├── Home.tsx
│   ├── Login.tsx
│   └── Signup.tsx
│
├── components/                       ← Shared reusable UI Wrapper components
│   └── ui/
│       ├── Button.tsx
│       ├── Input.tsx
│       └── Loader.tsx
│
├── features/                         ← Feature-based slices & components
│   └── auth/
│       ├── authSlice.ts              ← Redux slice
│       ├── AuthForm.tsx              ← Auth form component
│       └── authUtils.ts              ← Optional helper functions
│
├── services/                         ← RTK Query API files
│   └── authAPI.ts                    ← e.g., login, register endpoints
│
├── router/                           ← Routing logics and Browser router
│   └── router.tsx                    ← App route structure using createBrowserRouter
│
├── store/                            ← Redux store config
│   ├── index.ts                      ← Combine slices, apply middleware
│   └── rootReducer.ts                ← (Optional) Combine reducers
│
├── hooks/                            ← Custom reusable hooks
│   └── customHooks.ts                ← Custom Hooks if required
│
├── types/                            ← (Optional) Shared TypeScript types for 
|                                       the dependencies
│   └── index.ts
│
├── App.tsx                           ← App entry for child routes with Outlet
├── main.tsx                          ← Root renderer (RouterProvider)
|
├── test/                             ← Dedicated Test Folder
│   ├── App.test.tsx                  ← Unit test for App.tsx
│
│   ├── components/
│   │   └── ui/
│   │       ├── Button.test.tsx       ← Unit test for Button.tsx
│   │       └── Loader.test.tsx       ← Unit test for Loader.tsx
│
│   ├── features/
│   │   └── auth/
│   │       └── AuthForm.test.tsx     ← Unit test for AuthForm.tsx
│
│   └── pages/
│       └── Home.test.tsx             ← Unit test for Home page
```
## Backend

```
/server
│
├── /config               # App configuration (DB, environment, etc.)
│   └── db.js
│   └── env.js
│
├── /controllers          # Route logic and request handlers
│   └── authController.js
│   └── userController.js
│
├── /routes               # Route definitions
│   └── authRoutes.js
│   └── userRoutes.js
│
├── /services             # Reusable business logic (email, payment, etc.)
│   └── emailService.js
│
├── /middlewares          # Custom Express middlewares (auth, error handling, etc.)
│   └── authMiddleware.js
│   └── errorMiddleware.js
│
├── /utils                # Utility functions (validators, logger, etc.)
│   └── generateSitemap.js   
│
├── /public               # Static files (e.g., robots.txt, favicon)
│   └── robots.txt
│
├── index.js                # Main Express app setup
├── server.js               # App entry point
├── .env
├── package.json

```
