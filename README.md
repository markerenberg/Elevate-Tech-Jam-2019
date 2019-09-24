## Presenting the 3rd Place Winning Submission for Elevate Tech Jam 2019!

# Product Summary
Smart Queue is a mobile application that recommends the fastest way of getting service at a Rogers store. It factors in wait times and commute times to ensure that you have an accurate prediction of expected time to service.

# How Does It Work?
Smart Queue will use a customer's geolocation to find the closest Rogers stores around them. From here, we will use time-series modelling to predict expected wait times at each of the stores, and rank the stores in order of wait time + travel time.

# Model Implementation
The time-series model used in this project is an ARIMA model (Autoregressive Integrated Moving Average Model). It makes wait time predictions for each Rogers Store, and this information is combined with Google Maps travel times to give an expected Time To Service measures. 

Given a specific store and a desired time for service, our model uses the following primary inputs to predict expected wait times:
  1) Total number of customers at this store (according to total active devices sensed at the store's location).
  2) Total duration of time each customer spends at this store (measured by tracking the time a customer enters and leaves store's location).
  3) Total number of staff at this store (provided by Rogers).
  4) Average time spent with a customer (provided by Rogers).
Additional data is also used to model and forecast wait times, related to products/services offered at store.

# Business Value
Assuming Rogers has 1 million digital users , we can achieve $750M incremental gain in Customer Lifetime Value by improving churn rate even as much as 1%!

# Next Steps
Our next steps for this project are as follows:
  1) Optimize wait time model: Calibrate model after rollout and optimize across range of products/services offered at store.
  2) Reallocate staff in stores: Redistribute staff amongst stores to provide more service at stores with higher wait times.
  3) Integrate cross channel services: Predict wait times across other channels of service (phone, chat, etc.)
  
