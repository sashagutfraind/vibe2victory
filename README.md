# Vibe 2 Victory : a short guide to good software engineering with AI coders
by @sashagutfraind

## Background
Modern AI coders (Claude Code, Kiro, Codex, Cursor and others) easily exceed human coding ability
in dimensions such as 1. knowledge, 2. speed, and 3. availability.  The ability to deploy 
multiple cooperating agents means that large software stacks could be implemented by AI.
However, AI-implemented code is often unreliable, difficult to maintain, and fails to deliver.  
This guide discusses the root causes and some solutions.
It speaks both to human users (technical and non-technical) and to supervising AI agents.

## Major limitations of AI coding for your code
1. AI coders have biases from code they learned during training, which are subtly wrong in the your mission
2. AI coders do not know your users, business setting and implicit requirements
3. Knowledge about the code is not transferred to human maintainers, operators and users
4. Faulty instructions and specs will silently broke your solution
5. Software engineers work with more code, more isolation from others, with less hands-on practicing - degrading quality

## Solutions - principles
1. Focus your time on teaching your agent and the environment, not prompting and reviewing
2. Software is disposable
3. Agent time is cheap

## Solutions - setup
1. Background reading for AI: Prepare an extensive well-organized background reading for the agent ahead of implementation
2. Environment: Create a well-supplied and isolated environment, helping agents write software safer, faster and more autonomously
3. Spec: Write a detailed spec and review it with an agent for contradictions, risks and ambiguities
4. Architect if you can: technical users should spec the architecture and implementation, drawing on their experience and making the solution understandable to them
5. Non-technical users should spec the functional requirements precisely, to help the AI choose the correct architecture
6. Role playing: For implementation, provision multiple roles (e.g. planner, critic, data reader, implementer, reviewer, tester - see superpowers)

## Solutions - implementation and subsequent revision
1. Scaffolding: create a roadmap for development, building small testable modules
2. Prototype to reduce risk: build small prototypes to test assumptions about speed, data and apply the lessons
3. Extract the specs of the code, review it and do a clean room rebuild. Compare the solutions.

## Further reading
- https://github.com/obra/superpowers
- https://arps18.github.io/posts/claude-code-mastery/
 
