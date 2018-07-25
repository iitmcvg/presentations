@title[TF Estimators]

---

## What are Estimators?

Estimators encapsulate the following actions:

* training
* evaluation
* prediction
* export for serving/inferencwe

---

## Why Estimators?

Estimators provide the following benefits:

@ul

* Can run Estimator-based models on a local host or on a distributed multi-server environment without changing your model. Furthermore, you can run Estimator-based models on CPUs, GPUs, or TPUs without recoding your model.

* much easier to create models with Estimators than with the low-level TensorFlow APIs.

* Estimators are themselves built on tf.layers, which simplifies customization.

@ulend

+++


Estimators build the graph for you.
Estimators provide a safe distributed training loop that controls how and when to:
build the graph
initialize variables
start queues
handle exceptions
create checkpoint files and recover from failures
save summaries for TensorBoard
When writing an application with Estimators, you must separate the data input pipeline from the model. This separation simplifies experiments with different data sets.
