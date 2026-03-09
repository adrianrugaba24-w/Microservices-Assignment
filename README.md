# Microservices-Assignment
1. The Netflix Way: Breaking Things Into Pieces
Netflix runs its entire platform by splitting it into thousands of tiny, specialized programs called microservices. Each one does exactly one job — one handles subtitles, one tracks your "Continue Watching" list, one manages payments, and so on. They all talk to each other over a network.
The big advantage is resilience. If the subtitles service breaks, you can still watch your movie. And if millions of people log in at once, Netflix only needs to scale up the login service, not the entire system. For their 8,000+ engineers, it also means teams can work independently — fixing search won't accidentally break billing.
2. When Microservices Become Too Much
Some companies discovered that managing hundreds of tiny services can actually make things worse.
Amazon Prime Video was using microservices to check video quality. Every time one service finished a task, it had to send the result to the next one over the network. The data transfer costs and the waiting time were getting expensive and slow. Their fix: combine everything into one single program. The result — a 90% cost reduction and a faster system.
Segment had grown to over 140 microservices. To make one small change, engineers had to update 140 folders, test 140 systems, and deploy 140 times. It was exhausting. They merged everything back into one unified system, and their engineers could finally focus on building features again instead of fighting the infrastructure.
Neither approach is always better. Microservices work well for large teams and high-traffic apps that need flexibility. Monoliths are simpler, faster to build, and often the smarter choice for smaller teams. The real skill is knowing which one fits your situation.
