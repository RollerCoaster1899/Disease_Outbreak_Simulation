# Disease_Outbreak_Simulation

This code simulates a disease outbreak scenario and compares the outcomes between two scenarios: one without quarantine measures and another with quarantine measures. Here's an explanation of the code:

1. The `Person` class represents an individual in the population. Each person has attributes like `infected`, `recovered`, and `quarantined`, which indicate their health status. The `quarantine_probability` and `quarantine_infectiveness` parameters determine the likelihood of a person quarantining and the infectiveness of a person when quarantined, respectively.

2. The `OutbreakSimulator` class manages the simulation of the outbreak. It initializes the population of individuals with the specified parameters and infects the initially infected individuals. The `simulate` method runs the simulation for the given number of days and returns various percentages related to the health status of the population.

3. The `spread_infection` method spreads the infection from an infected person to susceptible individuals based on the infection rates. The infection rate is determined by the presence of quarantine measures and the infectiveness of the infected person.

4. The parameters for the simulation are defined, such as `population_size`, `initial_infected`, `no_quarantine_infection_rate`, `with_quarantine_infection_rate`, `recovery_rate`, `quarantine_probability`, `quarantine_infectiveness`, `simulation_days`, and `symptom_onset_day`.

5. Two instances of the `OutbreakSimulator` class are created: one for the scenario without quarantine (`simulator_no_quarantine`) and another for the scenario with quarantine (`simulator_with_quarantine`).

6. The `simulate` method is called on both simulators to obtain the percentages related to susceptible, infected, recovered, and quarantined individuals for each day of the simulation.

7. Finally, the results are plotted using `matplotlib`. The figure consists of four subplots: "Infected Percentage," "Recovered Percentage," "Quarantined Percentage," and "Susceptible Percentage." Each subplot shows the trends of the respective percentages over the simulation days for both the "No Quarantine" and "With Quarantine" scenarios.

By running this code, you can observe and compare the population dynamics, such as the spread of infection, recovery, and the impact of quarantine measures, in the two different scenarios.
