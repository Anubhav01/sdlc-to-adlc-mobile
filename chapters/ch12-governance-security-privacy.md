# Chapter 12: Governance, Security, and Privacy

## Why mobile raises the stakes
Apps hold personal data, run on devices users carry everywhere, and ship through stores with strict policies. Agent mistakes here become privacy incidents.

## Core risks
1. **Secrets leakage**: API keys, signing certificates, tokens pasted into prompts or committed.
2. **Unsafe code**: insecure storage, weak network settings, over-broad permissions.
3. **Data exposure**: sending user data or proprietary code to tools without approval.
4. **Prompt injection**: malicious text in issues, docs, or web pages that tries to steer an agent.
5. **Dependency risk**: agents adding unvetted libraries.
6. **Policy violations**: store rules, privacy declarations, and regional regulations.

## Controls
- Secrets in a vault, never in prompts; scan commits for secrets.
- Least privilege: agents get only the access the task needs.
- Approved-tools list and clear rules on what code or data may leave the company.
- Dependency review before adding any library.
- Treat external text read by agents as untrusted data, not instructions.
- Audit logs of agent actions.
- Human approval for sensitive areas: auth, payments, permissions, data deletion, release.

## Privacy checklist for mobile
Collect only needed data, request permissions at the moment of use, match store privacy declarations to actual behavior, and handle user deletion requests.

## Doubt Box
- **Is it safe to paste company code into an AI tool?** Only under your organization's approved tools and policies.
- **What is prompt injection?** Hidden instructions in content an agent reads that try to make it do something the user did not ask.
- **Who is responsible for compliance?** People, not agents.

## Try it
Write your team's list of "agents may never touch without human approval".
