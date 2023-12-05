| **Field** | Description | 
| ---- | ----- |
| API family name | Region User Count | 
| API family owner | China Unicom |
| Initial API Contributors | Fan Yang - China Unicom , Jin Xu - Huawei |
| API summary | **Description**     <br>  This API allows for the API Consumer to query the number of active users (i.e., excluding idle mode users). lin the specified area. The query area can be a circle or a polygon composed of longitude and latitude points.    <br>  **Use Cases**     <br>  User Story     1    : Emergency Response Planning    <br> - Role:  Emergency Response Coordinator    <br> - Context: During a natural disaster, such as a hurricane or earthquake, understanding the population density and distribution in affected areas is crucial for effective response planning.    <br>  - Goal: As an advertising platform administrator, I want to utilize the API to obtain the user count in a specific region, allowing me to enhance targeted advertising by tailoring campaigns to the user demographics in that area. By accessing the API, I can retrieve real-time user counts in these regions, allowing us to estimate the potential number of individuals affected and the resources needed for evacuation, medical aid, and support services.    <br>  User Story     2    : Targeted Advertising    <br> - Role: Advertising Platform Administrator    <br>  Goal: As an advertising platform administrator, I want to utilize the API to obtain the user count in a specific region, allowing me to enhance targeted advertising by tailoring campaigns to the user demographics in that area.     <br>  **Input**     <br>  - areaType    :Enumeration value: circle,Polygon    <br> - circleCenter     :The format is: longitude, latitude    <br>  Required when type is circle    <br>  - circleRadius :Unit: m. It is Required when type is circle    <br>  - pointListStr:The format is: Longitude 1, Latitude 1; Longitude 2, Latitude 2 @ Longitude 3, Latitude 3; Longitude 4 , Latitude 4. Longitude and Latitude are separated by English commas, multiple longitudes and latitudes are separated by English semicolons, and multiple regions are separated by the @ symbol    <br>  **Output**    <br>- userNum :the number of active users in the specified area. This number is provided is per serving operator in the area. <br>|
| Technical viability | This API is based on real-time location information expansion. It allows obtaining, on a per operator basis, the number of active users in a certain area based on their real-time location. |
| Commercial viability | For use in emergency rescue, disaster relief, intelligent transportation, smart tourism and other scenarios| 
| YAML code available? | NO<br>To be provided  |
| Validated in lab/productive environments? | YES<br>Available in China UniCom test environment |
| Validated with real customers? | YES<br>For emergency rescue use by the Blue Eye Emergency Rescue Platform |
| Validated with operators? | YES<br>Available for China Unicom in China |
| Supporters in API Backlog Working Group | China Unicom |