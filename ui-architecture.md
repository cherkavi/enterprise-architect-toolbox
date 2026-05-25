# UI architecture examples
## DDD style
* **Scalable Frontend Architecture slides:** https://slides.com/razazaidi/sfa/fullscreen
* **Beyond Console.log - Tracking vs Logging:** https://slides.com/razazaidi/tracking-vs-logging/fullscreen
* https://dev.to/huytaquoc/a-different-approach-to-frontend-architecture-38d4
* https://michalzalecki.com/elegant-frontend-architecture/

## The Multi-Tier Frontend Pipeline (BFF Pattern)
`FE UI ➔ FE NextJS ➔ BE` (utilizing Apollo & Next.js)
* **The Advice:** Avoid pointing the client-side UI directly at heavy, core backend services. Instead, utilize **Next.js** as a Backend-for-Frontend (BFF) layer to bridge the gap.
* **Best Practice:** Leverage **Apollo** (GraphQL) within the Next.js middle tier. This allows you to aggregate multiple backend API requests, orchestrate data efficiently, and serve clean, optimized payloads straight to the `FE UI`.

## Pragmatic Domain-Driven Design (DDD)
* **The Advice:** Don't treat Domain-Driven Design as a dogmatic, all-or-nothing rulebook. Treat DDD exactly as noted: a **pragmatic collection of tools and strategic advice**.
* **Key Takeaway:** Pick and choose the DDD patterns that solve your current scaling pain points (like bounded contexts and ubiquitous language) to untangle complex business logic, while ignoring the overhead for simpler CRUD features.

## The "New Modularity" Hierarchy
`New modularity: class ➔ package ➔ domain ➔ component`

* **The Advice:** Code encapsulation is shifting. Traditional architecture organized code by technical primitives (`classes` and `packages`). Modern, scalable architecture prioritizes **business-centric and functional boundaries**.
* **The Evolution:** * **Class & Package:** Micro-level, code-centric organization.
* **Domain:** The macro-level business boundary (organizing code by *what it does* for the business).
* **Component:** The self-contained, deployable unit of delivery (e.g., a micro-frontend or a isolated domain service).
* **Action Item:** Structure your repositories so that technical layers (like controllers or utilities) are nested *inside* Domain and Component boundaries, rather than the other way around.
