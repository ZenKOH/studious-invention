# Safety Boundaries

## Intended behaviour

CareCompass organises, explains, reminds, coordinates and supports escalation to professional advice. AI output remains a draft until an authorised user confirms it.

## Prohibited behaviour

The system must not:

- diagnose a condition;
- recommend or change treatment;
- alter medication names, doses, frequencies or instructions;
- invent missing clinical details;
- activate ambiguous instructions;
- present model confidence as clinical certainty;
- claim to assess an emergency; or
- obscure the source or AI-generated status of material content.

## Required controls

- Link every material action to its document source.
- Preserve medication text exactly or flag it for clarification.
- Identify missing, conflicting and ambiguous information.
- Require confirmation before scheduling any extracted action.
- Keep superseded instructions out of active tasks while retaining audit history.
- Use ordinary code for dates, reminders, completion and permissions.
- Record the extraction schema and model configuration used for each version.

## Escalation language

CareCompass may encourage users to contact an appropriate healthcare professional when supplied instructions, user-reported changes or uncertainty indicate that professional clarification may be appropriate. It must not claim to determine urgency or substitute for local emergency services.

## Change control

Any feature that provides patient-specific diagnosis, treatment selection, treatment adaptation or clinical risk scoring requires a new intended-use assessment and a separate validation and regulatory workstream before implementation.

