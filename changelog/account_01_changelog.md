# Changelog: account_01
**v1 → v2**

9 memo field(s) changed, 7 spec field(s) changed.

## Account memo changes (field-level diff)

**Field changed:** integration_constraints
- Old: ["create sprinkler jobs in ServiceTrade from the phone\u2014that's a constraint", "from the phone\u2014that's a constraint"]
- New: ["sprinkler jobs", "create sprinkler jobs in ServiceTrade from the agent"]

**Field changed:** emergency_definition
- Old: ["fire", "alarm", "emergency"]
- New: ["fire", "alarm", "emergency", "water leak"]

**Field changed:** notes
- Old: Extracted from demo call transcript (rule-based).
- New: Extracted from demo call transcript (rule-based). Updated from onboarding.

**Field changed:** office_address
- Old: 123 Main Street.
- New: 123 Main Street, Suite 100.

**Field changed:** emergency_routing_rules
- Old: ["our dispatch"]
- New: ["the phone tree", "Use phone tree / follow routing discussed."]

**Field changed:** call_transfer_rules.if_fails_say
- Old: If transfer fails we tell the caller someone will call back within an hour. We never create sprinkler jobs in ServiceTrade from the phone—that's a con
- New: If transfer fails after 60 seconds, dispatch must be notified. We retry twice.

Rep: ServiceTrade?

Client: Never create sprinkler jobs in ServiceTrad

**Field changed:** call_transfer_rules.timeouts
- Old: Not specified
- New: 60 seconds

**Field changed:** business_hours.timezone
- Old: Eastern
- New: EST

**Field changed:** business_hours.days
- Old: ["Monday", "Friday"]
- New: ["Monday to Fri"]

## Agent spec changes (field-level diff)

**Field changed:** version
- Old: v1
- New: v2

**Field changed:** key_variables.timezone
- Old: Eastern
- New: EST

**Field changed:** key_variables.business_hours
- Old: Monday, Friday 9 am-5 pm Eastern
- New: Monday to Fri 9 am-5 pm EST

**Field changed:** key_variables.office_address
- Old: 123 Main Street.
- New: 123 Main Street, Suite 100.

**Field changed:** key_variables.emergency_routing
- Old: our dispatch
- New: the phone tree; Use phone tree / follow routing discussed.

**Field changed:** fallback_protocol_if_transfer_fails
- Old: If transfer fails we tell the caller someone will call back within an hour. We never create sprinkler jobs in ServiceTrade from the phone—that's a con
- New: If transfer fails after 60 seconds, dispatch must be notified. We retry twice.

Rep: ServiceTrade?

Client: Never create sprinkler jobs in ServiceTrad

**Field changed:** system_prompt
- Old: You are the AI voice receptionist for Acme Fire Protection.
Your job is to answer incoming calls professionally, determine whether the caller's issue is emergency or non-emergency, collect the caller'
- New: You are the AI voice receptionist for Acme Fire Protection.
Your job is to answer incoming calls professionally, determine whether the caller's issue is emergency or non-emergency, collect the caller'
