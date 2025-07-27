# Claude Code Sub-Agents

A powerful collection of specialized AI coding assistants designed to streamline your development workflow. These sub-agents work within Claude Code to help you tackle specific programming tasks with expertise and precision.

## What Are Sub-Agents?

Think of sub-agents as your specialized coding teammates, each with their own expertise. Instead of asking a generalist AI to "do everything," these focused agents excel at specific tasks like writing specifications, reviewing code, or designing APIs. Each agent brings deep knowledge and best practices for their domain, making your development process more efficient and your code more professional.

**Why use sub-agents?**
- **Expertise**: Each agent is fine-tuned for specific tasks with domain-specific knowledge
- **Consistency**: Get reliable, repeatable results following industry best practices
- **Efficiency**: Skip the context-switching - work with agents who already understand your needs
- **Quality**: Benefit from specialized workflows and quality checks tailored to each task

## Quick Setup

Using these sub-agents in Claude Code is straightforward:

1. **Clone this repository** to your project workspace
2. **Navigate to the agent** you need in the `/agents` directory
3. **Copy the agent configuration** (usually found in the agent's README or `.md` file)
4. **Paste it into Claude Code** as a system prompt or project context
5. **Start working** with your specialized assistant!

Each agent directory contains everything you need: configuration files, usage examples, and detailed instructions.

## Available Sub-Agents

### Core Development Agents
- **spec-writer**: Creates comprehensive technical specifications and documentation
- **api-designer**: Designs REST APIs, GraphQL schemas, and service interfaces
- **frontend-developer**: Builds React components, responsive layouts, and UI optimization
- **code-reviewer**: Performs thorough code reviews with best practices and suggestions
- **test-generator**: Creates comprehensive test suites and quality assurance workflows

### Extended Capabilities
- **refactoring-specialist**: Modernizes codebases and improves architecture
- **database-architect**: Designs efficient database schemas and queries
- **deployment-engineer**: Handles CI/CD, containerization, and infrastructure
- **security-auditor**: Identifies vulnerabilities and implements security best practices

## Simple Example: Building a New API

Let's walk through creating a simple blog API using multiple sub-agents:

### Step 1: Write the Specification
```bash
# In Claude Code, load the spec-writer agent
@spec-writer "Create a specification for a blog API with posts, comments, and user management"
```

The spec-writer will generate detailed requirements, endpoints, data models, and acceptance criteria.

### Step 2: Design the API
```bash
# Load the api-designer agent with your spec
@api-designer "Design REST endpoints for this blog API specification: [paste spec here]"
```

You'll get properly designed endpoints, request/response schemas, status codes, and error handling.

### Step 3: Build the Frontend
```bash
# Use the frontend-developer for UI components
@frontend-developer "Create React components for displaying blog posts and comment threads"
```

Get modern, responsive React components with proper state management and styling.

### Step 4: Review and Test
```bash
# Have the code-reviewer examine your implementation
@code-reviewer "Review this blog API implementation for best practices and potential issues"

# Generate comprehensive tests
@test-generator "Create unit and integration tests for the blog API endpoints"
```

## Creative Workflow Example: E-commerce Platform

Here's how you might chain multiple agents for a more complex project:

### Planning Phase
1. **spec-writer** → Define requirements for an e-commerce platform
2. **database-architect** → Design the product catalog and user data schemas
3. **api-designer** → Create the service architecture and API contracts

### Development Phase
4. **frontend-developer** → Build the shopping cart and product listing components
5. **security-auditor** → Review payment handling and user authentication
6. **test-generator** → Create end-to-end tests for the shopping workflow

### Quality & Deployment
7. **code-reviewer** → Perform final code review and optimization suggestions
8. **deployment-engineer** → Set up CI/CD pipelines and production deployment

### Chaining Example
```bash
# Start with the spec
@spec-writer "E-commerce platform with product catalog, shopping cart, and payment processing"

# Pass the spec to the database architect
@database-architect "Design database schema for: [paste spec] - focus on scalability and performance"

# Use the API designer with both previous outputs
@api-designer "Create REST API design using this spec and database schema: [paste both]"

# Continue the chain with frontend development
@frontend-developer "Build React components for product browsing and cart management using this API: [paste API design]"
```

## Agent Invocation Patterns

### Single Agent Usage
```bash
# Direct task assignment
@agent-name "Specific task description with context"

# With file context
@agent-name "Review this code: [paste code] and suggest improvements"
```

### Multi-Agent Workflows
```bash
# Sequential: Pass output from one agent to the next
@spec-writer "Define requirements" → @api-designer "Design API" → @frontend-developer "Build UI"

# Parallel: Multiple agents working on different aspects
@frontend-developer "Build UI components" + @test-generator "Create test suite" + @deployment-engineer "Setup infrastructure"

# Iterative: Use agents to refine each other's work
@code-reviewer "Review implementation" → @refactoring-specialist "Optimize based on review" → @code-reviewer "Final review"
```

## Best Practices

- **Start with spec-writer** for any significant feature to establish clear requirements
- **Chain related agents** - pass outputs between agents for cohesive results
- **Use code-reviewer** as a final step to catch issues and improve quality
- **Combine multiple perspectives** - have different agents review the same code for comprehensive feedback
- **Keep context flowing** - reference previous agent outputs to maintain consistency

## Adding New Agents

Want to create a custom agent? Each agent follows a simple structure:

1. Create a new directory in `/agents/your-agent-name/`
2. Add a `README.md` with the agent's purpose and configuration
3. Include example usage and best practices
4. Add any specific prompts or configuration files
5. Update this main README to list your new agent

## Getting Started

Ready to supercharge your development workflow? 

1. Browse the `/agents` directory to see all available specialists
2. Pick an agent that matches your current task
3. Follow the setup instructions in the agent's README
4. Start building better code with specialized AI assistance!

Each agent is designed to work independently or as part of a larger workflow. Mix and match them based on your project needs, and don't hesitate to experiment with different combinations.

Happy coding! 🚀
