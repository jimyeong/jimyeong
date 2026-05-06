### Jimyeong Jung

**Full-stack engineer · IoT · Birmingham, UK**

I treat domain understanding as the part of the work that cannot be delegated. AI tools handle syntax and boilerplate; I guard the parts that decide what a system is actually *for* — what to keep, what to discard, where the failure modes are, and how the data flow reflects the real-world problem.

Currently building deeper ML expertise on top of a full-stack + IoT foundation. Open to **KTP positions in the UK** — UK Spouse Visa, no sponsorship required.

---

### Currently building

**[Lidless Platform](https://github.com/jimyeong/lidless-oracle)** — Multilingual, IoT-aware conversational system
`React Native` · `TypeScript` · `Apollo GraphQL` · `Python` · `Anthropic Claude API` · `PostgreSQL`

Distributed-by-design across four components (Controller / Hermes / Oracle / message broker), so a fault in one does not bring down the others. CQRS with outbox-inbox at the boundaries; GraphQL BFF gateway absorbing client divergence; tool schemas kept language-agnostic so the LLM serves whichever language the user is most comfortable in. Built with social housing tenants in mind, where first-language access matters.

**[OpsCheck](https://github.com/jimyeong/ops-check-service)** — Home IoT telemetry & data analysis system
`TypeScript` · `Fastify` · `MQTT (QoS-1)` · `Zigbee` · `RabbitMQ` · `PostgreSQL` · `AWS SNS` · `Python`

Zigbee chosen over Wi-Fi-only sensing because the data pipeline depends on the sensor layer not being the weakest link. Outbox + idempotent inbox + QoS-1 in combination — designed for a system where data preservation matters more than throughput. Notifications fire on **state transitions**, not raw thresholds: humidity must hold above 90% for an hour before the system shifts state and emits an alert. Behaviour modelled on how humidity actually behaves in the room.

**[Owlverload](https://github.com/jimyeong/inventory-ops-mobile)** — Inventory & expiry tracking, in daily use at a Birmingham supermarket
`React Native` · `TypeScript` · `Go` · `PostgreSQL` · `Cloudflare R2`

Sole-developer SDLC from Figma wireframes through App Store and Google Play deployment. Shipped v0 without wireframes to learn from real use; wireframed v1 after four months of observed friction. Wi-Fi dead zones in the shop were causing duplicate writes on reconnect, so an idempotency-key contract was paired with retry behaviour — interface and system contract designed together because the user's experience of failure depended on both.

---

### Stack I reach for

| Layer | Tools |
|---|---|
| **Languages** | TypeScript · Go · Python |
| **Frontend** | React · React Native |
| **Backend** | Node.js · Fastify · Apollo GraphQL |
| **Data** | PostgreSQL · RabbitMQ · MQTT · Zigbee |
| **ML / Data** | Pandas · Scikit-learn · Anthropic Claude API |
| **Infra** | Docker · Nginx · Cloudflare R2 · AWS (foundational) |

---

### How I work

- **Domain first.** Architecture serves the problem, not the other way around.
- **Failure modes are part of the design, not an afterthought.** Outbox patterns, idempotency keys, QoS settings — these are decisions about what the system is *allowed to lose*.
- **MVP first, wireframe later, when the problem is messy.** Real use produces friction that upfront design rarely captures.
- **Honest postmortems over polished retrospectives.** I write down the wrong hypotheses, not just the right diagnosis.

---

### Elsewhere

- 💼 [LinkedIn]([https://linkedin.com/in/jimyeong](https://www.linkedin.com/in/jimyeong-jung-725a9223a/) — UK job search & engineering notes
- 🧮 [LeetCode](https://leetcode.com/u/idjjm92/)
- 📚 Reading log on Instagram (DM for the handle)

📍 Birmingham, UK · 🗣 English / 한국어
