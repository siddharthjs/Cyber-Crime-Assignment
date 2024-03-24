# Cyber Crime Assignment

City, University of London
INM446 Cyber Crime and Socio-technical risk (PRD2 A 2023/24)
Nouf A Almosaied
230044740
Coursework 1 (30% of total marks)
31st of March, 2024
Dr. Lorenzo Strigini

## Introduction

The vast categorization of cyber crimes, including fraud, offenses against the person, illegal access, and data interference, among others, suggests that any security measure must be dynamic and adaptable. This diversity in threats necessitates that both the "Clean Desks" policy and the sophisticated entrance gate must not be static defenses but part of a continuously evolving security posture that anticipates and adapts to new forms of cybercrime.

## Expected Utility Calculation

The expected utility (EU) for the intruder is calculated by summing the products of the utilities of all outcomes and their respective probabilities. The utility of each outcome is determined by the gain or loss to the intruder.

### Probabilities:

1. **P_enter:** Probability of entering the restricted area = 50% or 0.5
2. **P_not_challenged_looking:** Probability of not being challenged while looking for target rooms = 90% or 0.9
3. **P_steal_loot:** Probability of stealing loot without being noticed = 50% or 0.5
4. **P_not_challenged_exit:** Probability of not being challenged on exit = 99% or 0.99
5. **P_caught_stealing:** Probability of being caught red-handed while stealing = 10% or 0.1
6. **P_challenged:** Probability of being challenged = 10% or 0.1
7. **P_convinces:** Probability of convincing if challenged = 50% or 0.5
8. **P_challenged_exit:** Probability of being challenged on way out = 1% or 0.01

### Utilities:

1. **U_success:** Utility of success (leaving with the loot) = +120,000 pounds
2. **U_failure:** Utility for failure (not obtaining loot or caught but not convicted) = -1,000 pounds
3. **U_heavy_punishment:** Utility for heavy punishment (caught with loot) = -100,000 pounds
4. **U_light_punishment:** Utility for light punishment (arrested without loot) = -10,000 pounds

### Calculations for Each Path:

1. **Success Path:** The intruder enters, is not challenged, steals the loot, and exits without challenge.  
   Calculation: P_enter * P_not_challenged_looking * P_steal_loot * P_not_challenged_exit * U_success = 0.5 * 0.9 * 0.5 * 0.99 * 120,000 = 26,730 pounds
2. **Failed at Stealing, Exits Without Being Noticed:** The intruder enters, is not challenged, fails to steal, and exits without challenge.  
   Calculation: P_enter * P_not_challenged_looking * (1 - P_steal_loot) * U_failure = 0.5 * 0.9 * (1 - 0.5) * -1,000 = -225 pounds
3. **Caught Red-handed While Stealing:** The intruder is caught in the act.  
   Calculation: P_enter * P_caught_stealing * U_heavy_punishment = 0.5 * 0.1 * -100,000 = -5,000 pounds
4. **Challenged and Convinces:** The intruder is challenged but convinces the challenger and proceeds to steal the loot.  
   Calculation: P_enter * P_challenged * P_convinces * P_steal_loot * U_success = 0.5 * 0.1 * 0.5 * 0.5 * 120,000 = 1,500 pounds
5. **Challenged, Fails to Convince, Arrested Without Loot:** The intruder is challenged, fails to convince, and is arrested without the loot.  
   Calculation: P_enter * P_challenged * (1 - P_convinces) * U_light_punishment = 0.5 * 0.1 * (1 - 0.5) * -10,000 = -250 pounds
6. **Exits With Loot, Challenged on Way Out, Convinces:** The intruder exits with the loot, is challenged on the way out, but convinces the challenger.  
   Calculation: P_enter * P_steal_loot * P_challenged_exit * P_convinces * U_success = 0.5 * 0.5 * 0.01 * 0.5 * 120,000 = 150 pounds
7. **Exits With Loot, Challenged on Way Out, Fails to Convince, Arrested With Loot:** The intruder exits with the loot, is challenged on the way out, fails to convince, and is arrested with the loot.  
   Calculation: P_enter * P_steal_loot * P_challenged_exit * (1 - P_convinces) * U_heavy_punishment = 0.5 * 0.5 * 0.01 * (1 - 0.5) * -100,000 = -125 pounds

### Total Expected Utility:

The total expected utility combines the utilities of all possible paths to provide an overall expected outcome for the intruder's decision to attack. Given the calculations above, the intruder's total expected utility is:  
26,730 (Success Path) − 225 (Failed Stealing) − 5,000 (Caught Red-handed) + 1,500 (Challenged and Convinces) − 250 (Challenged, Fails) + 150 (Exit, Convinces) − 125 (Exit, Fails) = 22,780 pounds.

## Decision According to Normative Theory

Given that the expected utility for the intruder is positive (22,780 pounds), according to normative decision theory, the rational choice for the intruder would be to "attack" rather than "do not attack," assuming their cost for not attacking is zero. This conclusion is drawn because a positive expected utility indicates that the overall outcome of the action (attacking) is favorable from the intruder's perspective.

## Option 1: Implementing 'Clean Desks' Policy

### Impact:

- Halves the probability of successfully stealing loot (from 50% to 25%).

### Cost:

- £12,000 per month in lost productivity.

### Expected Utility Calculations:

For each option, we need to recalculate the intruder's expected utility and the company's expected financial impact. The calculations will be based on the probabilities and utilities provided in the original question and the modified probabilities for each option.

We'll calculate the intruder's expected utility and the company's expected monthly cost for both options. Remember, the company's monthly cost includes the cost of the security measure plus any expected losses from successful intrusions. We'll also compare these to the intruder's original expected utility to see if their rational decision (attack or not attack) changes.

#### Recalculated Expected Utility:

1. **Success Path:**
   Calculation: P_enter * P_not_challenged_looking * P_steal_loot_clean_desks * P_not_challenged_exit * U_success = 0.5 * 0.9 * 0.25 * 0.99 * 120000 = 13,365 pounds

2. **Failed at Stealing, Exits Without Being Noticed:**
   Calculation: P_enter * P_not_challenged_looking * (1 - P_steal_loot_clean_desks) * U_failure = 0.5 * 0.9 * 0.75 * -1000 = -337.5 pounds

3. **Caught Red-handed While Stealing:**
   Calculation: P_enter * P_caught_stealing * U_heavy_punishment = 0.5 * 0.1 * -100000 = -5,000 pounds

4. **Challenged and Convinces, then Steals:**
   Calculation: P_enter * P_challenged * P_convinces * P_steal_loot_clean_desks * U_success = 0.5 * 0.1 * 0.5 * 0.25 * 120000 = 750 pounds

5. **Challenged, Fails to Convince, Arrested Without Loot:**
   Calculation: P_enter * P_challenged * (1 - P_convinces) * U_light_punishment = 0.5 * 0.1 * 0.5 * -10000 = -250 pounds

6. **Exits With Loot, Challenged on Way Out, Convinces:**
   Calculation: P_enter * P_steal_loot_clean_desks * P_challenged_exit * P_convinces * U_success = 0.5 * 0.25 * 0.01 * 0.5 * 120000 = 75 pounds

7. **Exits With Loot, Challenged on Way Out, Fails to Convince, Arrested With Loot:**
   Calculation: P_enter * P_steal_loot_clean_desks * P_challenged_exit * (1 - P_convinces) * U_heavy_punishment = 0.5 * 0.25 * 0.01 * 0.5 * -100000 = -62.5 pounds

### Total Expected Utility for 'Clean Desks' Policy:

EU_clean_desks = 13,365 - 337.5 - 5,000 + 750 - 250 + 75 - 62.5 = 8,540 pounds.

## Option 2: Installing Sophisticated Entrance Gate

### Impact:

- Reduces the probability of an intruder entering the restricted area by 75% (from 50% to 12.5%).

### Cost:

- £3,000 per month, including gate costs and lost productivity.

### Recalculated Expected Utility:

1. **Success Path:**
   Calculation: P_enter_sophisticated_gate * P_not_challenged_looking * P_steal_loot * P_not_challenged_exit * U_success = 0.125 * 0.9 * 0.5 * 0.99 * 120000 = 6,682.5 pounds

2. **Failed at Stealing, Exits Without Being Noticed:**
   Calculation: P_enter_sophisticated_gate * P_not_challenged_looking * (1 - P_steal_loot) * U_failure = 0.125 * 0.9 * 0.5 * -1000 = -56.25 pounds

3. **Caught Red-handed While Stealing:**
   Calculation: P_enter_sophisticated_gate * P_caught_stealing * U_heavy_punishment = 0.125 * 0.1 * -100000 = -1,250 pounds

4. **Challenged and Convinces, then Steals:**
   Calculation: P_enter_sophisticated_gate * P_challenged * P_convinces * P_steal_loot * U_success = 0.125 * 0.1 * 0.5 * 0.5 * 120000 = 375 pounds

5. **Challenged, Fails to Convince, Arrested Without Loot:**
   Calculation: P_enter_sophisticated_gate * P_challenged * (1 - P_convinces) * U_light_punishment = 0.125 * 0.1 * 0.5 * -10000 = -62.5 pounds

6. **Exits With Loot, Challenged on Way Out, Convinces:**
   Calculation: P_enter_sophisticated_gate * P_steal_loot * P_challenged_exit * P_convinces * U_success = 0.125 * 0.5 * 0.01 * 0.5 * 120000 = 37.5 pounds

7. **Exits With Loot, Challenged on Way Out, Fails to Convince, Arrested With Loot:**
   Calculation: P_enter_sophisticated_gate * P_steal_loot * P_challenged_exit * (1 - P_convinces) * U_heavy_punishment = 0.125 * 0.5 * 0.01 * 0.5 * -100000 = -31.25 pounds

### Total Expected Utility for Sophisticated Entrance Gate:

EU_sophisticated_gate = 6,682.5 - 56.25 - 1,250 + 375 - 62.5 + 37.5 - 31.25 = 5,695 pounds.

## Comparative Analysis

### Reduction in Expected Utility:

Both security measures effectively reduce the expected utility for potential intruders, albeit to different extents. The sophisticated entrance gate leads to a more considerable decrease in expected utility compared to the 'Clean Desks' policy. This suggests that making entry more challenging has a more substantial deterrent effect than making the final step of the attack (stealing loot undetected) harder. The sophisticated entrance gate addresses the threat at an earlier stage by preventing entry. The 'Clean Desks' policy, though impactful, relies on intruders bypassing initial security layers.

### Cost-Benefit Consideration:

The sophisticated entrance gate offers a more favorable cost-benefit ratio. Its lower monthly cost (£3,000) and significant impact on reducing intrusion probability make it a cost-effective deterrent. In contrast, the 'Clean Desks' policy, despite its higher cost (£12,000 per month), provides broader cultural security benefits that are harder to quantify financially.

### Long-Term Implications:

The entrance gate is a one-time investment with ongoing minimal costs, potentially offering enduring deterrence with little need for further intervention. The 'Clean Desks' policy requires continuous enforcement and cultural adaptation, which may vary in effectiveness over time.

## Conclusion and Recommendation

Considering the direct impact on preventing unauthorized access, lower ongoing costs, and significant reduction in the expected utility for potential intruders, installing a sophisticated entrance gate emerges as the more strategic choice. This measure effectively decreases the likelihood of intrusion attempts by addressing the challenge at the point of entry, offering a strong deterrent effect that is both efficient and financially sensible.

While the 'Clean Desks' policy undeniably fosters a security-conscious workplace culture, its higher cost and dependency on consistent employee compliance make it a less favorable primary deterrent strategy. Nonetheless, it could serve as a valuable complementary measure to reinforce the overall security posture.

In light of these analyses, the recommendation is to prioritize the installation of the sophisticated entrance gate as the primary measure to deter potential intruders, potentially supported by the 'Clean Desks' policy for a layered defense strategy.

