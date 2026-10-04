# Exchange Protocol

This protocol defines the lightweight lifecycle for public-safe exchange items.

Public exchange status does not equal canonical status.

An item becomes canonical only after authorized reconciliation into the relevant canonical system.

## States

- `NEW`: submitted or created, not yet triaged.
- `TRIAGED`: reviewed enough to identify purpose and next owner/path.
- `IN-REVIEW`: under human, AI, or reviewer evaluation.
- `READY-FOR-RECONCILIATION`: ready for an authorized worker to reconcile into canonical memory.
- `RECONCILED`: reconciled into the relevant canonical system, with receipt or pointer preserved.
- `DEFERRED`: intentionally postponed.
- `REJECTED`: reviewed and not accepted for reconciliation or further action.

## Item Metadata

Use this header for exchange items:

```text
ID:
CREATED:
CREATED-BY:
WORK-TYPE:
TARGET:
SENSITIVITY:
STATUS:
CANONICAL-DESTINATION:
RELATED-SOURCES:
```

Sensitivity values:

- `PUBLIC`
- `PUBLIC-SAFE`
- `REVIEW-REQUIRED`

Anything actually sensitive must not be committed here.

## Reconciliation

Agents without canonical write access may still contribute public-safe work here or authorized collaborative work in Drive.

When canonical write access is unavailable:

- keep the work bounded;
- mark uncertainty clearly;
- avoid claiming canonical truth;
- use `CANONICAL VERIFICATION PENDING` where private verification is required;
- prepare handoff material for a Human or authorized agent.

Important decisions should be reconciled promptly. Routine exchange material may be reconciled periodically.

No scheduled job is created by this V1 protocol.

## Reconciliation Receipt

After reconciliation, preserve traceability with a receipt when possible:

```text
Exchange Item ID:
Original location:
Canonical destination:
Canonical commit / artifact:
Reconciled by:
Reconciled date:
Result:
Notes:
```

Do not delete history merely because reconciliation completed.
