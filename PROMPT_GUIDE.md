# E-Commerce Project: Prompt Engineering Guide

This document contains the prompts used to generate the codebase and documentation for this e-commerce project. Use these as reference for maintenance or to understand the project's structure and functionality.

## Project Initialization

### Core Project Structure
```
Create a full-stack e-commerce application with the following structure:
- Client (Next.js 13+ with App Router)
  - Authentication (login/register)
  - Product listing and search
  - Shopping cart functionality
  - User profile and orders
- Server (Node.js/Express)
  - RESTful API endpoints
  - JWT authentication
  - SQLite database with Sequelize ORM
  - File upload support
```

## Frontend Prompts

### Authentication System
```
Create a complete authentication system with:
1. Login page with email/password
2. Registration form with validation
3. Protected routes
4. JWT token management
5. User context using React Context API
6. Form handling with react-hook-form
7. Error handling and loading states
```

### Product Pages
```
Generate product listing pages with:
- Grid/List view toggle
- Category filters
- Search functionality
- Pagination
- Responsive design using Tailwind CSS
- Loading skeletons
- Error boundaries
```

### Shopping Cart
```
Implement shopping cart functionality with:
- Add/remove items
- Quantity adjustment
- Cart persistence using localStorage
- Real-time price calculation
- Checkout button that redirects to login if not authenticated
```

## Backend Prompts

### API Endpoints
```
Create RESTful API endpoints for:
- Authentication (register, login, profile, logout)
- Products (CRUD operations)
- Categories
- Orders
- Users
Include proper validation, error handling, and JWT authentication middleware.
```

### Database Models
```
Design database models for:
1. User (id, name, email, password, role, timestamps)
2. Product (id, name, description, price, image, category, stock, timestamps)
3. Order (id, userId, total, status, shippingAddress, timestamps)
4. OrderItem (id, orderId, productId, quantity, price)
5. Category (id, name, description)

Include model associations and validations.
```

## Deployment Prompts

### Vercel Deployment
```
Generate configuration for deploying the Next.js frontend to Vercel including:
- vercel.json configuration
- Environment variables setup
- Build and output settings
- CORS configuration
- Cache headers
```

### Backend Deployment
```
Create deployment configuration for the Node.js backend including:
- PM2 ecosystem file
- Environment variables
- Database connection pooling
- Production error handling
- Logging setup
```

## Documentation Prompts

### API Documentation
```
Generate OpenAPI/Swagger documentation for all API endpoints including:
- Request/response schemas
- Authentication requirements
- Query parameters
- Example requests and responses
- Error codes and messages
```

### README.md
```
Create a comprehensive README with:
- Project overview
- Features list
- Tech stack
- Installation instructions
- Environment setup
- Available scripts
- Deployment guide
- Contributing guidelines
```

## Testing Prompts

### Unit Tests
```
Generate unit tests for:
- Authentication service
- Product service
- Cart functionality
- API endpoints
- Utility functions
```

### E2E Tests
```
Create end-to-end test scenarios for:
- User registration flow
- Login/logout
- Product search and filtering
- Add to cart and checkout
- Order history
```

## Maintenance & Updates

### Code Quality
```
Add configuration for:
- ESLint with React/TypeScript rules
- Prettier for code formatting
- Husky for pre-commit hooks
- Lint-staged for staged file checking
```

### Performance Optimization
```
Implement optimizations for:
- Image optimization
- Code splitting
- Lazy loading
- Bundle size reduction
- Caching strategies
```

## Security Prompts

### Authentication
```
Enhance security with:
- Rate limiting
- CSRF protection
- XSS prevention
- Secure cookie settings
- Password hashing with bcrypt
- JWT token refresh mechanism
```

### API Security
```
Implement security best practices:
- Input validation
- SQL injection prevention
- Request size limits
- CORS configuration
- Security headers
- Rate limiting
```

## CI/CD

### GitHub Actions
```
Create GitHub Actions workflows for:
- Automated testing on push/pull requests
- Linting and type checking
- Build verification
- Deployment to staging/production
- Dependency updates
```

## Monitoring & Analytics

### Error Tracking
```
Integrate error tracking with:
- Sentry for frontend errors
- Winston for server-side logging
- Error boundary components
- Error reporting middleware
```

### Analytics
```
Add analytics for:
- User behavior tracking
- Performance metrics
- Error rates
- Feature usage
- Conversion funnels
```

---

This prompt guide serves as a living document. Update it as you add new features or make significant changes to the codebase.
