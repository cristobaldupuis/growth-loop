# Right On Call: claims

Ground truth is `cristobaldupuis/voice-agent`, file `docs/CLAIMS.md`. This table was checked against it on 2026-10-11. Re-check at the start of every `/draft`, because capabilities move into and out of production within a week.

| Topic | Safe to say | Do not say | Source |
|---|---|---|---|
| Language | English and French. The agent answers in the language the caller starts in. | Any other language as live. The website itself is English only. | Language |
| AI disclosure | If a caller asks whether it is a person or an AI, it always says it is an AI assistant. A recording notice is spoken when the shop has one set. | Anything implying callers cannot tell it is an AI. | AI disclosure; Call recording disclosure |
| Booking | Offers only times your calendar actually shows. Sends a confirmation text after the call. | Invents availability. Reschedules or cancels for you: it books a new visit and texts the shop to cancel the old one. | Invented availability; Rescheduling and cancelling |
| Diagnosis and pricing | Never diagnoses a cause. Never quotes a repair or parts price. Only states the shop's diagnostic fee. | Free diagnostic (use missed-call audit). Any repair quote. | Diagnosis / repair pricing |
| Fridge and freezer lead time | Respects per-item minimum lead times set by the shop. | Same-day fridge or freezer booking. The default minimum is 5 days even if the caller says urgent. | Scheduling lead time |
| Calendars | Cal.com and Calendly are live. | Direct Google Calendar integration. | Calendar integrations |
| Job and CRM systems | Jobber is live (creates client and job, does not assign a tech). Zoho CRM and Zoho Invoice are live. Housecall Pro works on the MAX plan, on request. | Listed in the Jobber Marketplace. ServiceTitan, AppFolio, Buildium or Workiz as live (no adapters exist, on request only). | Jobber; Housecall Pro; Other adapters |
| Handoff to a person | Texts your on-call number with the caller's name, number and reason. | Transfers calls to your team. Always reaches a person. Live transfer is not live anywhere. | Live transfer; SMS destination |
| Photos | Callers can reply by text with a photo of the appliance. | Anything about photo diagnosis. Use sparingly until the photo read is re-tested live. | Photo intake |
| Reminders and weekly summary | Nothing yet. | Day-before reminders and the Monday ROI digest. Built, but the scheduler is not running, so they are not live. | LAUNCH_CHECKLIST task 37 |
| Booking by text | Nothing yet. | Booking by text as a live feature until the pilot has it switched on. | Booking by text (SMS agent) |
| Returning callers | Recognizes returning customers (the name must match) and offers their last address. | Remembers history. Knows who is calling by number alone. Customer memory (not live). | Returning-caller recognition; Customer memory |
| Texts | Confirmation texts to Canadian numbers deliver. | Texts reach US numbers. | Booking confirmation |
| Data retention | Recordings kept about 14 days. Transcripts kept 12 months, then anonymised. | We delete your data after a year (say anonymised). No identifier can ever survive the scrub. | Retention rows |
| Proof | A live pilot with an appliance repair shop in London, Ontario. | Recovered-job counts, revenue results, the client's name or a quote without their OK. Any HVAC or plumbing results: no non-appliance partner has billed. | Verticals / taxonomy |
| After hours and calculator | Answers after hours and texts the on-call number. Calculator figures are a planning estimate. | Wakes your tech or full emergency dispatch (after-hours behaviour is still being defined on the pilot). Presenting calculator dollars as results. | LAUNCH_CHECKLIST task 4; site calculator |

## Known site issues (not for posts)

- The Managed plan card on rightoncall.com lists ServiceTitan, AppFolio and Buildium job sync. `voice-agent/docs/CLAIMS.md` says no adapters exist for these, so the site copy should say on request.
