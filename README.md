# Android App: Voyager v2
It is an android app that calculates the optimal (shortest) route for visiting all entered stop points. That is, it solves the classic "Traveling Salesman Problem (TSP)". Examples: travellers visiting different sightseeing landmarks, explorers planning road trips, realtors scheduling open house visits, businesses (e.g., couriers/delivery people) optimizing their service routes. 

You may download it through the Play Store, https://play.google.com/store/apps/details?id=com.sensis.voyager.app

## Getting Started
1. Open IntelliJ or Android Studio
2. Import Project
3. Import project from external model -> Gradle
4. Use defaults

## Notes
1. The app has not been tested for production usage and not intented to be used by serious users (e.g. couriers). If you are looking for a more stable/battle-proof app, please check out the previous version "Voyager: Route Planner" in the Play Store, https://play.google.com/store/apps/details?id=com.sensis.voyager
2. Optimal route calculation is NOT done based on data from the Google directions service. It simply uses the direct distance between two stops (by the Haversine algorithm) and no traffic condition is taken into account.
3. ButterKnife is used extensively, and unfortunately that requires proper handling of unbinding. To ease this a little, there are helper base classes in the ioc package.
