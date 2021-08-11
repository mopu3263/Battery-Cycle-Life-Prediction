This project shows how to predict the remaining cycle life of a fast charging Li-ion battery using linear regression, a supervised machine learning algorithm and compare the result with PyTorch deep learning model. Lithium-ion battery cycle life prediction using a physics-based modelling approach is very complex due to varying operating conditions and significant device variability even with batteries from the same manufacturer. For this scenario, machine learning based approaches provide promising results when sufficient test data is available. Accurate battery cycle life prediction at the early stages of battery life would allow for rapid validation of new manufacturing processes. It also allows end-users to identify deteriorated performance with sufficient lead-time to replace faulty batteries. To this end, only the first 100 cycles based features are considered for predicting remaining cycle life and the prediction error is shown to be about 10%.

Dataset:
The dataset contains measurements from moer than 1000 lithium-ion cells with nominal capacity of 1.1 Ah and a nominal voltage of 3.3 V under various charge and discharge profiles. For this example, the data is curated to only contain a subset of measurements relevant to the features being extracted. Training data contains measurements from 500 cells, validation data contains measurements from 300 cells and the test data contains measurements from 300 cells. Data for each cell is stored in a structure, which includes the following information:

Descriptive data: Cell barcode, charging policy, cycle life

Per-cycle summary data: Cycle number, discharge capacity, internal resistance, charge time

Data collected within a cycle: Time, temperature, linearly interpolated discharge capacity, linearly interpolated voltage
