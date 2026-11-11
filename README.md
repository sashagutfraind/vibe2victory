# Vibe 2 Victory : a flash guide to good software engineering with AI coders
by @sashagutfraind

## Background
Modern AI coding agents (Claude Code, Kiro, Codex, Cursor and others) easily exceed human coding ability in dimensions such as 1. knowledge, 2. speed, and 3. availability.  Already large software stacks could be implemented by AI agent teams. However, in practice AI-implemented code is often unreliable, difficult to maintain, and fails to deliver - why and what could be done?  

This flash guide discusses the root causes and some solutions. It speaks both to human users (technical and non-technical) and to supervising AI agents.

## Major limitations of AI coding for your software
1. Agents do not magically know your users, business setting and implicit requirements
2. Agents have biases from code they learned from other codebases, which are subtly wrong for your mission
3. Faulty instructions and specs will silently break your solution
4. Over time your agent-written software will grow in size, complexity and rot the architecture - making fixes and fault recovery harder
5. Your code will be trapped in a local minimum because agents prefer inline fixes over risky large-scale refactoring
6. Knowledge about your code will not be transferred to human maintainers, operators and users;  their coding skills will degrade from disuse

## Solutions - principles
1. Agent engineering over software engineering: focus your time on engineering your agents and their environment - not building software
2. Software architecting over code writing: Problem knowledge and good architecture are the assets - software is disposable and agent time is cheap
3. Frontier agents are powerful but not error-free: expect errors, hallucinations, and context degradation
4. Prompting and reviewing diffs is low-value labor - ask yourself: how can you fix your system?
5. Keep human the boss - continuously learn new software engineering skills

## Solutions - setup
1. Background reading for agents: Prepare an extensive well-organized background reading for the agent ahead of implementation
2. Environment: Create a well-resourced and isolated environment, helping agents write software safer, faster and more autonomously
3. Spec: Write a detailed spec and review it with an agent for contradictions, risks and ambiguities
4. Architect if you can: technical builders should spec the architecture and interfaces, drawing on their experience and making the solution understandable to themselves
5. Non-technical users should spec the functional requirements precisely to help the agents choose the correct architecture
6. Role playing agents: create multiple agentic roles (e.g. planner, critic, data reader, implementer, reviewer, tester - see superpowers)

## Solutions - implementation and subsequent revision
1. Roadmap: create a roadmap for development; use previous stacks as reference and scaffold for next iterations
2. Prototype to reduce risk: build small prototypes to test assumptions about speed, data and apply the lessons
3. Cleanroom replication: extract the specs of the code, review it for errors, and do a clean room rebuild. Compare the solutions.
4. Contract design: codify interfaces between components to reduce complexity and architecture rot


## Further reading
- https://github.com/obra/superpowers
- https://arps18.github.io/posts/claude-code-mastery/
 
