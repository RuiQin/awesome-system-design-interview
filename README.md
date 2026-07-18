# Awesome System Design Interview

> 60 in-depth, worked system design interview guides — functional and non-functional requirements, capacity estimations, data models, API design, high-level architecture, and deep dives. Free to read.

Each guide has a fully interactive version — Mermaid diagrams, hover-to-define glossary terms, and a companion AI **voice** mock interviewer — at **[Scale Interview](https://scaleinterview.ai/learn)**.

## Contents

- [Easy](#easy)
- [Medium](#medium)
- [Hard](#hard)

## Easy

- **[Design a Unique ID Generator](https://scaleinterview.ai/learn/system-design/unique-id-generator)** — Design a unique ID generator at scale with Snowflake — time-sortable 64-bit IDs, clock skew, sequences, and no single point of failure.
- **[Design a URL Shortener](https://scaleinterview.ai/learn/system-design/url-shortener)** — A full system design walkthrough of a URL shortener like Bitly — requirements, estimations, data model, API, architecture, and code generation.
- **[Design Consistent Hashing](https://scaleinterview.ai/learn/system-design/consistent-hashing)** — Consistent hashing explained — the hash ring, virtual nodes for balance, replication, and minimal key movement when nodes join or leave
- **[Design Pastebin](https://scaleinterview.ai/learn/system-design/pastebin)** — Design Pastebin — create and read text pastes by unique key, keep large blobs in object storage, expire with TTL, scale reads via caching and CDN

## Medium

- **[Design a Collaborative To-Do List](https://scaleinterview.ai/learn/system-design/collaborative-todo-list)** — Design a real-time collaborative to-do list — WebSocket sync, item-level conflict resolution with CRDTs, reordering by order key, and offline merge.
- **[Design a Distributed Cache](https://scaleinterview.ai/learn/system-design/distributed-cache)** — Distributed in-memory cache design like Redis — consistent hashing, virtual nodes, replication, LRU eviction, cache-aside, and invalidation.
- **[Design a Distributed Job Scheduler](https://scaleinterview.ai/learn/system-design/job-scheduler)** — Design a distributed job scheduler — schedule jobs at a time, at-least-once execution, recurring cron jobs, retries and worker leasing.
- **[Design a Distributed Key-Value Store](https://scaleinterview.ai/learn/system-design/key-value-store)** — Durable distributed key-value store — consistent-hashing partitioning, N-way replication, tunable quorum reads/writes, vector-clock conflict fixes
- **[Design a File Storage & Sync Service](https://scaleinterview.ai/learn/system-design/file-storage)** — A system design walkthrough of a file storage and sync service like Dropbox — chunked uploads, content-addressed deduplication, and multi-device sync.
- **[Design a Hotel Reservation System](https://scaleinterview.ai/learn/system-design/hotel-reservation)** — Design a hotel reservation system — search available rooms by date range, book without overbooking, the availability calendar, plus cancellations
- **[Design a Likes System](https://scaleinterview.ai/learn/system-design/likes-system)** — System design of a like/unlike system at scale — idempotent likes, sharded counters for hot keys, has-liked lookups, and eventual consistency.
- **[Design a Local Delivery Service](https://scaleinterview.ai/learn/system-design/local-delivery)** — Design DoorDash — courier matching timed to prep time, real-time tracking with ETA, and an order lifecycle across customer, restaurant, and courier.
- **[Design a Metrics Monitoring & Alerting System](https://scaleinterview.ai/learn/system-design/metrics-monitoring)** — Design metrics monitoring & alerting — time-series ingestion, TSDB rollups, cardinality, low-latency dashboards, and a reliable alert pipeline
- **[Design a News Aggregator](https://scaleinterview.ai/learn/system-design/news-aggregator)** — Design a news aggregator like Google News — crawl sources, cluster duplicate articles into one story, rank and personalize, serve a fresh feed
- **[Design a Notification System](https://scaleinterview.ai/learn/system-design/notification-system)** — A system design walkthrough of a multi-channel notification system — fan-out to push/email/SMS, at-least-once delivery, idempotency, and retries.
- **[Design a Price Tracker](https://scaleinterview.ai/learn/system-design/price-tracker)** — A system design walkthrough of a price tracker like CamelCamelCamel — crawling at scale, time-series price history, and efficient alert evaluation.
- **[Design a Real-Time Gaming Leaderboard](https://scaleinterview.ai/learn/system-design/gaming-leaderboard)** — Design a real-time gaming leaderboard — rank millions of players with sorted sets, get-rank, top-N and around-me queries, hot keys, and sharding.
- **[Design a Web Crawler](https://scaleinterview.ai/learn/system-design/web-crawler)** — Design a web crawler at scale — URL frontier and politeness, robots.txt, bloom-filter dedup, canonicalization, and distributed fetcher workers.
- **[Design an A/B Testing System](https://scaleinterview.ai/learn/system-design/ab-testing)** — Design an A/B testing platform — variant assignment, low-latency config delivery, exposure and outcome logging, and honest statistical significance
- **[Design an Ad Click Aggregator](https://scaleinterview.ai/learn/system-design/ad-click-aggregator)** — System design of an ad click aggregator at scale — stream processing, windowed aggregation with watermarks, exactly-once counting, and hot ads.
- **[Design an API Rate Limiter](https://scaleinterview.ai/learn/system-design/rate-limiter)** — A system design walkthrough of a distributed API rate limiter — algorithms (token bucket, sliding window), atomic Redis counting, and placement.
- **[Design an Email Service](https://scaleinterview.ai/learn/system-design/distributed-email)** — Design an email service — sending and receiving mail over SMTP, mailbox storage with threads and labels, full-text search, and spam filtering
- **[Design Chess.com](https://scaleinterview.ai/learn/system-design/online-chess)** — System design of an online chess platform like Chess.com — Elo matchmaking, real-time moves over WebSocket, and server-authoritative clocks.
- **[Design LeetCode](https://scaleinterview.ai/learn/system-design/leetcode)** — Design a LeetCode online judge — submitting code, sandboxed execution against test cases, a judging queue and worker fleet, contests and ranking.
- **[Design Nearby Friends (Real-Time Location) System Design](https://scaleinterview.ai/learn/system-design/nearby-friends)** — Design Nearby Friends — real-time location, geohash proximity cells, and pub/sub fan-out over the friend graph to show friends nearby, live
- **[Design Reddit (Forum & Comments) System Design](https://scaleinterview.ai/learn/system-design/reddit)** — Design Reddit — model nested comment trees, rank posts and comments by time-decayed votes, and serve read-heavy subreddit and home feeds at scale.
- **[Design Search Autocomplete](https://scaleinterview.ai/learn/system-design/search-autocomplete)** — Design search autocomplete — prefix trie, top-K per node, frequency + recency ranking, sharded read path, sub-100ms suggestions at Google scale
- **[Design Short Video Recommendation & Ranking](https://scaleinterview.ai/learn/system-design/short-video-recommendation)** — Design a short-video recommender — two-tower retrieval, a ranking model on watch-time + engagement, cold start, delayed labels, low-latency serving
- **[Design Slack](https://scaleinterview.ai/learn/system-design/slack)** — Design Slack team chat — workspaces and channels, real-time message delivery over WebSockets, presence, unread state, and searchable message history
- **[Design Spotify (Music Streaming) System Design](https://scaleinterview.ai/learn/system-design/spotify)** — Design Spotify music streaming — audio delivery with prefetch and offline sync, catalog and playlists, and Discover-Weekly recommendations.
- **[Design Strava](https://scaleinterview.ai/learn/system-design/strava)** — Design Strava — recording GPS activities, matching a track to segments with a spatial index, and per-segment leaderboards
- **[Design Tinder](https://scaleinterview.ai/learn/system-design/tinder)** — Design Tinder — billions of swipes at scale, mutual-match detection on the write path, geospatial candidate generation, and match notifications
- **[Design Yelp](https://scaleinterview.ai/learn/system-design/yelp)** — Design Yelp — nearby-business proximity search over a geospatial index (geohash/quadtree), ratings and reviews, and a read-heavy serving path

## Hard

- **[Design a Chat App](https://scaleinterview.ai/learn/system-design/chat-app)** — A system design walkthrough of a chat app like WhatsApp — real-time delivery over persistent connections, message ordering, and read receipts.
- **[Design a Delayed Payment Scheduler](https://scaleinterview.ai/learn/system-design/delayed-payment-scheduler)** — System design of a scheduled/delayed payment system — durable scheduling, exactly-once execution under retries, and hot wall-clock minutes.
- **[Design a Digital Wallet](https://scaleinterview.ai/learn/system-design/digital-wallet)** — Design a digital wallet — balances backed by a double-entry ledger, idempotent transfers, atomic debit/credit, and no double-spend under concurrency
- **[Design a Distributed Message Queue](https://scaleinterview.ai/learn/system-design/distributed-message-queue)** — Design a distributed message queue (Kafka-style) — the append-only log, partitioning, replication, consumer groups, and delivery semantics.
- **[Design a Friend-Played Game Counter](https://scaleinterview.ai/learn/system-design/friend-game-counter)** — Design a friend-played game counter — friends-who-played and live player counts via social-graph set intersection, fan-out, hot keys, near-real-time
- **[Design a GPU Credits System](https://scaleinterview.ai/learn/system-design/gpu-credits)** — Design a GPU credits system — metering GPU usage at scale, a credit ledger and billing, plus quota enforcement and cutoff when credits run out.
- **[Design a Matchmaking Service](https://scaleinterview.ai/learn/system-design/matchmaking-service)** — System design of a multiplayer matchmaking service — skill-based matching, queue pools, fairness vs wait-time, and game-server allocation.
- **[Design a News Feed](https://scaleinterview.ai/learn/system-design/news-feed)** — A full system design walkthrough of a social news feed like Facebook or Twitter — requirements, estimations, data model, API, fan-out, and ranking.
- **[Design a Payment System](https://scaleinterview.ai/learn/system-design/payment-system)** — System design of a payment system like Stripe — idempotent exactly-once charges, authorize-then-capture, and money/order consistency.
- **[Design a Remote IDE](https://scaleinterview.ai/learn/system-design/online-ide)** — System design of a cloud IDE like Replit or Codespaces — isolating untrusted code, fast workspace cold start, and persisting the filesystem.
- **[Design a Ride-Sharing Service](https://scaleinterview.ai/learn/system-design/ride-sharing)** — A system design walkthrough of a ride-sharing service like Uber — matching riders to nearby drivers, geospatial indexing, and location pings.
- **[Design a Stock Exchange](https://scaleinterview.ai/learn/system-design/stock-exchange)** — Design a stock exchange — limit order book, price-time-priority matching engine, microsecond latency, and event-sourced durability with recovery
- **[Design a Ticket Booking System](https://scaleinterview.ai/learn/system-design/ticket-booking)** — A system design walkthrough of a ticket booking system like Ticketmaster — seat holds, double-booking, waiting rooms, and idempotent payment.
- **[Design a Video Streaming Service](https://scaleinterview.ai/learn/system-design/video-streaming)** — A system design walkthrough of a video streaming service like YouTube — resumable upload, the transcoding pipeline, and adaptive streaming.
- **[Design Amazon](https://scaleinterview.ai/learn/system-design/amazon)** — Design Amazon — product catalog and search, cart, and order placement with inventory that never oversells via reservations, idempotency, and a saga.
- **[Design an Ads Ranking System](https://scaleinterview.ai/learn/system-design/ads-ranking)** — Design an ads ranking system — candidate ad scoring, multi-task engagement models, calibration for the auction, and delayed-conversion labels
- **[Design an Object Storage Service](https://scaleinterview.ai/learn/system-design/s3-object-storage)** — Design an S3 object store — buckets and objects, a metadata service mapping keys to chunks, 11-nines durability via replication or erasure coding
- **[Design an Online Auction](https://scaleinterview.ai/learn/system-design/online-auction)** — Design an online auction — bidding under concurrency, highest-bid consistency, a timed close with anti-snipe, and live price updates to watchers
- **[Design ChatGPT](https://scaleinterview.ai/learn/system-design/llm-inference)** — A system design walkthrough of an LLM inference service like ChatGPT — token streaming over SSE, GPU scheduling, continuous batching, and KV cache.
- **[Design Facebook Live Comments](https://scaleinterview.ai/learn/system-design/fb-live-comments)** — Design Facebook Live comments — real-time comment fan-out to millions of viewers on one live video, ingest spikes, sampling, and WebSockets at scale
- **[Design Facebook Post Search](https://scaleinterview.ai/learn/system-design/fb-post-search)** — Facebook post search — inverted index, document sharding, ranking by relevance and recency, real-time post indexing at scale
- **[Design Google Docs](https://scaleinterview.ai/learn/system-design/google-docs)** — System design of a collaborative editor like Google Docs — concurrent-edit conflict resolution (OT vs CRDT), live cursors, and offline sync.
- **[Design Google Maps](https://scaleinterview.ai/learn/system-design/google-maps)** — Design Google Maps — road-network shortest-path routing via contraction hierarchies, live-traffic ETA from GPS probes, and quadtree map tiles
- **[Design Instagram](https://scaleinterview.ai/learn/system-design/instagram)** — Design Instagram — media upload to blob store + CDN, hybrid fan-out feed with celebrity problem, follow graph, and like counters at scale
- **[Design Robinhood](https://scaleinterview.ai/learn/system-design/robinhood)** — Design Robinhood — placing orders routed to an exchange, real-time market-data fan-out over WebSockets, and portfolio and positions consistency
- **[Design Top K YouTube Videos (Heavy Hitters) System Design](https://scaleinterview.ai/learn/system-design/youtube-top-k)** — Design top-K trending YouTube videos — streaming heavy hitters with a count-min sketch, tumbling and sliding time windows, and exact reconciliation.
- **[Design Twitter (X) System Design](https://scaleinterview.ai/learn/system-design/twitter)** — Design Twitter (X) — hybrid home-timeline fan-out, the celebrity problem, a precomputed timeline cache, and real-time trending topics

## About Scale Interview

[Scale Interview](https://scaleinterview.ai) is an AI-powered platform for real-time **voice** system design interview practice. Instead of just reading a solution, you talk through the problem out loud with an AI interviewer that asks real follow-ups, challenges your tradeoffs, and pushes on scale — then gives you structured feedback afterward.

- 🎙️ **Voice-first mock interviews** — explain out loud, like the real thing
- 🔀 **Adaptive follow-ups** — probes your weak spots, not a fixed script
- 📊 **Structured feedback** — requirements, tradeoffs, communication, depth
- 📚 **60 in-depth guides** — every one above, practiceable live

**[Try a free interview → https://scaleinterview.ai/mock](https://scaleinterview.ai/mock)**

---

Guides maintained by **[Scale Interview](https://scaleinterview.ai)**. Want a topic added? Open an issue.

<!-- Generated from the Scale Interview guide catalog. Do not edit by hand. -->
