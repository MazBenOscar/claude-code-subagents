# Shadcn-UI MCP Rule Set

This document defines the comprehensive rules and best practices for using the shadcn/ui MCP server effectively in frontend development projects.

## 1. Discovery Phase Rules

### 1.1 Component Discovery
- Always start with `list_components()` to understand available components
- Use `get_component_metadata(name)` to understand component requirements and dependencies
- Check `get_directory_structure()` to understand the project layout
- Identify existing components before creating new ones

### 1.2 Block Discovery
- Use `list_blocks()` to discover pre-built UI patterns and page sections
- Prioritize blocks over individual components for complex layouts
- Verify block compatibility with project requirements

### 1.3 Dependency Analysis
- Check component dependencies before implementation
- Identify required peer dependencies (React, Tailwind CSS, etc.)
- Verify version compatibility across the component ecosystem

## 2. Planning Phase Rules

### 2.1 Component Selection Strategy
- Prefer blocks for page-level layouts and complex sections
- Use individual components for specific UI elements
- Plan component composition hierarchy before implementation
- Consider accessibility requirements from the start

### 2.2 Implementation Order
- Install base dependencies first
- Implement foundational components before complex ones
- Plan for responsive design across all breakpoints
- Consider dark mode support in component selection

### 2.3 Architecture Planning
- Design component props interfaces early
- Plan state management strategy
- Consider component reusability across the application
- Plan for testing and documentation

## 3. Implementation Phase Rules

### 3.1 Component Installation
- Use `get_component(name)` to fetch individual components
- Use `get_block(name)` to fetch complete UI blocks
- Follow the exact installation instructions provided
- Verify all dependencies are installed correctly

### 3.2 Code Integration
- Maintain consistent naming conventions
- Follow TypeScript best practices when applicable
- Ensure proper import/export structure
- Maintain clean separation of concerns

### 3.3 Customization Guidelines
- Use CSS custom properties for theme customization
- Leverage Tailwind CSS utilities for styling modifications
- Maintain component accessibility features
- Document any custom modifications clearly

## 4. Page-Specific Implementation Rules

### 4.1 Landing Pages
- Prioritize hero sections and call-to-action blocks
- Use marketing-focused components (testimonials, features, pricing)
- Ensure mobile-first responsive design
- Optimize for conversion and user engagement

### 4.2 Dashboard Pages
- Use data visualization components (charts, tables, cards)
- Implement proper navigation and sidebar components
- Consider real-time data updates and loading states
- Prioritize information hierarchy and readability

### 4.3 Form Pages
- Use form components with built-in validation
- Implement proper error handling and feedback
- Ensure keyboard navigation and accessibility
- Consider multi-step form patterns when needed

### 4.4 E-commerce Pages
- Use product display and shopping cart components
- Implement filtering and search functionality
- Consider payment and checkout flow components
- Optimize for mobile commerce experiences

## 5. Error Handling Rules

### 5.1 MCP Server Errors
- Always handle MCP server connection failures gracefully
- Implement fallback strategies for missing components
- Log MCP server errors for debugging
- Provide meaningful error messages to users

### 5.2 Component Errors
- Implement error boundaries for component failures
- Handle missing props and invalid data gracefully
- Provide loading states and error feedback
- Test error scenarios thoroughly

### 5.3 Dependency Errors
- Verify all required dependencies are installed
- Handle version conflicts appropriately
- Provide clear installation instructions for missing dependencies
- Test component functionality after dependency updates

## 6. Optimization Rules

### 6.1 Performance Optimization
- Implement lazy loading for heavy components
- Use React.memo() for expensive re-renders
- Optimize bundle size by importing only needed components
- Implement proper code splitting strategies

### 6.2 Accessibility Optimization
- Ensure all components meet WCAG 2.1 AA standards
- Test with screen readers and keyboard navigation
- Implement proper ARIA attributes and landmarks
- Provide alternative text and descriptions

### 6.3 SEO Optimization
- Use semantic HTML elements appropriately
- Implement proper heading hierarchy
- Ensure content is crawlable and indexable
- Optimize for Core Web Vitals metrics

## 7. Versioning and Maintenance Rules

### 7.1 Version Management
- Track shadcn/ui component versions used
- Document any custom modifications made
- Plan for component updates and migrations
- Test compatibility after version updates

### 7.2 Documentation Requirements
- Document component usage and customizations
- Maintain component inventory and dependencies
- Create usage examples and best practices
- Keep implementation notes for future reference

### 7.3 Testing Requirements
- Implement unit tests for custom component logic
- Test responsive design across devices
- Verify accessibility compliance
- Test integration with other system components

## 8. Quality Assurance Rules

### 8.1 Code Quality
- Follow consistent coding standards and linting rules
- Implement proper TypeScript types when applicable
- Maintain clean and readable code structure
- Use meaningful variable and function names

### 8.2 Design System Compliance
- Ensure components align with design system guidelines
- Maintain consistent spacing, typography, and colors
- Follow established patterns and conventions
- Document any deviations from standards

### 8.3 Cross-Browser Compatibility
- Test components across major browsers
- Implement fallbacks for unsupported features
- Verify consistent rendering and functionality
- Address browser-specific issues promptly

## 9. Security Considerations

### 9.1 Input Validation
- Sanitize all user inputs in form components
- Implement proper validation for data types
- Prevent XSS and injection attacks
- Use secure authentication patterns

### 9.2 Data Handling
- Implement secure data transmission practices
- Protect sensitive information in components
- Follow privacy and compliance requirements
- Audit third-party component dependencies

## 10. Deployment and Production Rules

### 10.1 Build Optimization
- Optimize component bundles for production
- Implement proper caching strategies
- Minimize CSS and JavaScript output
- Test production builds thoroughly

### 10.2 Monitoring and Analytics
- Implement error tracking for component failures
- Monitor component performance metrics
- Track user interactions and engagement
- Set up alerts for critical issues

By following these comprehensive rules, developers can ensure effective, maintainable, and high-quality implementation of shadcn/ui components through the MCP server interface.
