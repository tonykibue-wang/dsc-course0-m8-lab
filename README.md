# Aviation Accident Analysis

Project overview
This project analyzes the data of recorded aviation incidents since 1983 to determine the relationship between the aircraft make/model and the selected conditions of the incidents. The results of this analysis are intended to be used as a basis for research into aircraft categories that deserve particular attention, not to rank planes according to their level of safety.
The analysis focuses on two outcomes:
• Serious/fatal injury rate: the recorded number of seriously or fatally injured occupants divided by the estimated number of occupants in an accident.
• Aircraft destruction rate: the proportion of reported cases in which the aircraft was recorded as destroyed.

Main findings
• Outcomes vary between aircraft makes/models. Some have lower average serious/fatal injury fraction, some has lower observed destruction fraction; both measures should be considered.
• Analysis divides small and large aircraft based on recorded occupants as a proxy. Enables general comparison but misclassification of aircraft due to absence of reliable recorded certified seating capacity in the dataset.
• Model-level distribution plots demonstrate that, within a given make/model, accident outcomes can vary considerably. Mean summarizes the distribution but does not capture variation in outcomes.
• Weather condition and phase of flight are investigated as factors associated with injury severity and destruction. Results are suggestive but cannot imply causation. Further analysis is required to determine if there is an association.

Limitations
• Accident records are not exposure data. The dataset has no total flights, departures, or flight hours per make/model, so the analysis estimates outcomes of recorded accidents, not the chance per flight / flight hour.
• Occupant count is a proxy for size category. The small/large split was made using estimated recorded occupants, not manufacturer-certified passenger capacity.
• Missing injury counts can bias results. Wherever a missing injury count would be necessary to perform a calculation, that value is replaced with zero, and a "missing-count" indicator is retained for that observation. This can cause some calculated injury fractions to be lower than they would be if the missing information were known.
• Sample sizes can bias results. Small-sized samples have greater variance in their mean. The notebook applies thresholds for minimum sample size, but these do not eliminate uncertainty or bias.

Conclusion
This project can serve as an example of an efficient way to clean the data on aviation accidents, engineer features to characterize accident outcomes, and evaluate aircraft groups’ performance using summary statistics and visualization. The results can be utilized to shortlist the aircraft types for further analysis. To make more accurate conclusions on aircraft safety, it would be reasonable to take into account additional information, such as the size of the fleet, aircraft age and configuration, number of flights, and details on each accident’s investigation.
