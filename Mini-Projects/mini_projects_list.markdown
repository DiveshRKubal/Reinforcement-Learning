# List of Mini-Projects

**1. Dynamic Pricing Engine (E-Commerce)**

**Business Context:** Amazon and Flipkart use RL to adjust product prices in real time based on demand, competitor pricing, and inventory levels.
 **What to Build:** Simulate a simple e-commerce environment where a Q-Learning agent learns to set optimal prices to maximize revenue. Use a custom OpenAI Gym environment with states like inventory level and demand signal.

Data - https://www.kaggle.com/datasets/suddharshan/retail-price-optimization





**2. Personalized Ad Bidding System (Digital Marketing)**

**Business Context:** Real-time bidding (RTB) platforms use RL to decide how much to bid for ad impressions per user to maximize ROI.
 **What to Build:** Train a Multi-Armed Bandit or DQN agent on a simulated ad auction environment. States = user profile features; actions = bid amount buckets; reward = click/conversion signal.

Data - https://ailab.criteo.com/download-criteo-1tb-click-logs-dataset/



**3. Intelligent Chatbot with RL-Based Dialog Management**

**Business Context:** Companies like Salesforce and Zendesk embed RL into customer support bots to optimize multi-turn conversation flows.
 **What to Build:** Build a goal-oriented chatbot where a PPO agent manages dialog states (greet → clarify → resolve → close) trained using simulated user interactions and reward = task completion.

Data - https://github.com/budzianowski/multiwoz



**4. Stock Portfolio Management Agent (FinTech)**

**Business Context:** J.P. Morgan uses deep RL for algorithmic trading and optimal trade execution strategies.
 **What to Build:** Use historical stock data (e.g., NSE/BSE via yfinance) to train a DQN agent that learns buy/hold/sell decisions. Reward = daily portfolio return. Use the FinRL library as a starter scaffold.

Data - https://www.kaggle.com/datasets/alincijov/trading



**5. Traffic Signal Optimization (Smart City / IoT)**

**Business Context:** Smart traffic management systems use RL to minimize vehicle wait times at intersections — deployed in cities like Hangzhou, China.
 **What to Build:** Use the **SUMO traffic simulator** with a Deep Q-Network agent that controls signal phases. State = queue lengths per lane; reward = reduction in cumulative waiting time.

Data - https://eclipse.dev/sumo/



**6. Cloud Resource Auto-Scaler (DevOps / Cloud IT)**

**Business Context:** AWS, Azure, and GCP use RL-based autoscaling to dynamically provision compute resources based on workload patterns, reducing costs.
 **What to Build:** Simulate a cloud server environment where an RL agent decides to scale up/down based on CPU utilization and request queue. Reward = SLA compliance minus provisioning cost.

Data - https://github.com/google/cluster-data



**7. Warehouse Robot Path Planner (Logistics / Supply Chain)**

**Business Context:** Amazon Robotics and Covariant deploy RL-powered robots in fulfillment warehouses for navigation and pick-and-place tasks.
 **What to Build:** Use a grid-world environment (or MiniGrid from Gym) where an agent learns shortest-path navigation to shelves while avoiding obstacles. Reward = speed + energy efficiency.

Data - https://github.com/Farama-Foundation/Minigrid



**8. Adaptive Learning Platform (EdTech)**

**Business Context:** EdTech platforms use RL to personalize quiz difficulty and content sequencing based on learner performance — a growing area with huge investment potential.
 **What to Build:** Build a student simulation where an RL agent selects the next question difficulty (easy/medium/hard). State = student's recent performance history; reward = improvement in test scores over episodes.

Data - https://www.kaggle.com/c/riiid-test-answer-prediction/data



**9. Energy Consumption Optimizer (Sustainability / IT Infra)**

**Business Context:** Google reduced data center cooling costs by **40%** using DeepMind's RL-based energy management system.
 **What to Build:** Simulate a data center with variable server load and cooling units. Train an RL agent to schedule cooling and load balancing. Reward = energy saved while maintaining temperature thresholds.

Data - https://archive.ics.uci.edu/ml/datasets/individual+household+electric+power+consumption

Data - https://energyplus.net/



**10. Fraud Detection with RL-Based Sampling (Banking / FinSec)**

**Business Context:** Banks use RL to decide which transactions to flag for review, balancing detection accuracy with analyst workload.
 **What to Build:** Formulate fraud review as a sequential decision problem. Train a Bandit or DQN agent on a publicly available fraud dataset (e.g., Kaggle Credit Card Fraud) to learn an optimal review policy. Reward = true positive detections minus false positive cost.

Data - https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud

Data - https://www.kaggle.com/datasets/imaadmahmood/fraud-guard-synthetic-2025





**11. Hospital Appointment Scheduler (HealthTech)**

**Business Context:** Hospitals use RL to optimize appointment slot allocation, reduce patient wait times, and maximize doctor utilization — a critical IT problem in healthcare operations.
 **What to Build:** Simulate a clinic with doctor slots and incoming patient requests. A Q-Learning agent learns to assign appointments based on urgency, specialty, and availability. Reward = patient wait time minimized + slot utilization maximized.

Data - https://www.kaggle.com/datasets/joniarroba/noshowappointments



**12. Network Intrusion Detection System (Cybersecurity)**

**Business Context:** Microsoft Azure's Project Narya uses RL to predict and prevent service disruptions and security threats in real time.
 **What to Build:** Use the NSL-KDD or CICIDS dataset. Train a DQN agent that observes network traffic features and decides: allow / flag / block. Reward = true threat detections minus false alarms. Implement in Python with gym and scikit-learn.

Data - https://www.unb.ca/cic/datasets/nsl.html

Data - https://www.unb.ca/cic/datasets/ids-2018.html



**13. Supply Chain Inventory Optimizer (Retail / Logistics)**

**Business Context:** Companies like Walmart and Maersk use RL agents to dynamically manage stock replenishment across warehouses to prevent overstock or stockouts.
 **What to Build:** Build a multi-echelon inventory simulation (supplier → warehouse → store). Train a PPO agent to decide reorder quantities at each step. Reward = holding cost + stockout penalty minimized.

Data - https://www.kaggle.com/datasets/harshsingh2209/supply-chain-analysis

Data - https://www.kaggle.com/c/m5-forecasting-accuracy/data



**14. Personalized News Feed Curator (Media / SaaS)**

**Business Context:** Platforms like LinkedIn News and Inshorts use RL-based recommendation to balance content recency, diversity, and user engagement.
 **What to Build:** Model the feed as a multi-armed bandit or contextual bandit problem. States = user reading history embeddings; actions = article categories; reward = simulated click-through or reading time. Use Thompson Sampling or LinUCB.

Data - https://msnews.github.io/

Data - https://www.kaggle.com/c/outbrain-click-prediction



**15. Autonomous IT Helpdesk Ticket Router (IT Service Management)**

**Business Context:** ServiceNow and Jira use intelligent routing to auto-assign support tickets to the right team based on load, skills, and SLA deadlines — reducing MTTR (Mean Time to Resolve).
 **What to Build:** Simulate a helpdesk with multiple teams and incoming tickets. An RL agent learns to route tickets optimally. State = ticket category + team availability; reward = SLA compliance rate.

Data - https://www.kaggle.com/datasets/deddy/it-service-management-tickets

Data - https://huggingface.co/github-issues/datasets



**16. Drug Dosage Optimization Agent (Pharma / MedTech)**

**Business Context:** RL is used in clinical decision support to personalize drug dosages (e.g., insulin or chemotherapy) based on patient vitals, reducing adverse events.
 **What to Build:** Using the SimGlucose or a custom simulated patient environment, train a DDPG agent to recommend insulin dosage per time step. Reward = blood glucose maintained in the safe range.

Data - https://github.com/jxx123/simglucose

Data - https://pubmed.ncbi.nlm.nih.gov/33584164/



**17. Smart Grid Demand Response Controller (Energy / Sustainability)**

**Business Context:** Utility companies deploy RL to dynamically shift electricity loads during peak demand periods, integrating renewable sources seamlessly.
 **What to Build:** Simulate a grid with solar/wind variability and consumer demand curves. Train an RL agent (SAC) to control load-shedding and storage dispatch. Reward = grid stability score minus energy waste.

Data - https://archive.ics.uci.edu/ml/datasets/Appliances+energy+prediction



**18. Autonomous SQL Query Optimizer (Database / Backend Engineering)**

**Business Context:** Database engines like PostgreSQL and Google Spanner are exploring RL to learn better query execution plans, outperforming hand-crafted heuristics.
 **What to Build:** Simulate a query plan search space using the Join Order Benchmark dataset. Train a tree-based RL agent (using DQN or Monte Carlo Tree Search) to select join orderings. Reward = estimated query execution cost reduction.

Data - https://github.com/gregrahn/join-order-benchmark

Data - https://www.tpc.org/tpch/



**`9. Multi-Agent Ride-Hailing Dispatcher (MaaS / Transport Tech)**

**Business Context:** Ola and Uber use multi-agent RL to coordinate fleets of drivers across city zones, minimizing passenger wait time and driver idle time simultaneously.
 **What to Build:** Simulate a city grid with driver agents and random ride requests. Use **MARL (Multi-Agent RL)** with shared or independent Q-networks. Reward = average pickup time minimized across all agents. Use the PettingZoo library for multi-agent environments.

Data - https://www.nyc.gov/site/tlc/about/tlc-trip-record-data.page