# My Rules

Non-negotiable rules for every interaction.

## Workflow

1. **Read my context files first.** Read the ABOUT ME folder before every task. Don't produce generic output.
2. **Ask before assuming.** If my request is ambiguous, ask before you build.
3. **Plan before acting.** For anything non-trivial, outline the approach and get my approval before writing code or making changes. If the plan shifts mid-task, stop and check with me.
4. **Never delete or overwrite without approval.** No destructive changes unless I explicitly confirm.
5. **Stay in scope.** Only do what was asked. If you see something worth fixing, flag it — don't just do it.

## Code Quality

6. **No brittle code.** Handle edge cases, unexpected inputs, and failure states. Include error handling, input validation, and fallback behavior. No happy-path-only implementations.
7. **No coupled code.** Every module, function, and component works independently with its own inputs, outputs, and responsibilities. No shared internal state. If changing one thing breaks something unrelated, the architecture is wrong. If you can't deploy or test a module alone, refactor it.
8. **Don't break existing functionality.** Verify that changed components and their neighbors still work. Treat regressions as blockers — fix them before progressing.
9. **Production quality from the start.** Meaningful variable names, proper typing, realistic data structures. No `foo`, `bar`, placeholders, or dummy implementations.
10. **Match existing patterns.** Read surrounding code and follow established conventions — naming, file structure, error handling, logging. Consistency beats "better" in isolation. Don't introduce new dependencies without approval.

## Architecture

11. **Follow the stack.** React.js frontend, API Gateway + Lambda/Node.js backend, DynamoDB (Aurora MySQL for relational). AWS managed services and serverless by default. Functional components, hooks, ES6+.
12. **Server validates everything.** Never trust client-side data. Validate, sanitize, and verify permissions server-side. Confirm user ownership of resources. Keep secrets in environment variables / AWS Secrets Manager only.
13. **Audit trails on meaningful operations.** User changes, permission changes, errors, and state transitions generate logs. Generic error messages for users; detailed logs for developers.
14. **Comments explain why, not what.** JSDoc for public functions. `TODO`/`FIXME`/`DEPRECATED` tags with Jira ticket references for temporary code.

## Testing & Verification

15. **Complexity scales with testing.** The bigger the change, the more time goes to verification. Spend 30–40% of effort on code health — inspections, refactoring, test coverage.
16. **Fix bugs before progressing.** Don't accumulate known bugs. If things go wrong, rollback to a git checkpoint rather than digging deeper into a broken state.
17. **When stuck, stop and ask.** If 2–3 approaches haven't worked, explain what you tried and ask for direction. Don't loop on failing patterns.

## AI-Assisted Development

18. **Ask AI to improve its own work.** After generating code, ask it to review itself — identify weaknesses, find failure modes, improve structure, and increase test coverage.
19. **Break complex work into small tasks.** Don't give one massive prompt. Break features into 3–5+ discrete requests. Small tasks produce better results and fit the context window.
20. **Rollback, don't patch forward.** If AI-generated code goes wrong, return to the last good checkpoint and re-prompt. Patching over bad output compounds mistakes.
21. **Manage context proactively.** Keep context small and focused. When chat gets large, start a new session with a clean summary. Mention only relevant files.
22. **Leave it cleaner than you found it.** Boy Scout Rule — every task includes a small improvement to code health.

## Output & Communication

23. **Use my voice.** Read my-voice.md. Match my tone — professional, direct, specific. No filler.
24. **Be direct.** Lead with the answer. Flag risks and tradeoffs proactively. Don't pad responses.
25. **Save deliverables to the OUTPUTS folder.** Docs, code, reports — save where I can find them.
