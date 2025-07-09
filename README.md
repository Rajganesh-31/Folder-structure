# Folder structure

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
|   |                                   with lazy loading and protected routes
│   └── router.tsx                    
|
├── store/                            ← Redux store config
│   ├── index.ts                      ← Combine slices, apply middleware
│   └── rootReducer.ts                ← (Optional) Combine reducers
│
├── hooks/                            ← Custom reusable hooks
│   ├── customHooks.ts                ← Custom Hooks if required
│                                      
│
├── App.tsx                           ← App entry point child routes with outlet
|                                       
|                                        
├── main.tsx                          
└── types/                            ← (Optional) Shared TypeScript types for 
    |                                   the dependencies
    └── index.ts

/test                                   ← ✅ Dedicated test folder
│
├── App.test.tsx                        ← Unit test for App.tsx
│
├── components/
│   └── ui/
│       ├── Button.test.tsx             ← Unit test for Button.tsx
│       └── Loader.test.tsx             ← Unit test for Loader.tsx
│
├── features/
│   └── auth/
│       └── AuthForm.test.tsx           ← Unit test for AuthForm.tsx
│
├── pages/
│   └── Home.test.tsx                   ← Unit test for Home page
```
