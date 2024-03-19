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

