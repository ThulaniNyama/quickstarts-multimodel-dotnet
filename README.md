# Multi-Model QuickStart for .NET Code Sample

This code shows multi-model access to InterSystems IRIS data platform in .NET.

The sample is used in the [Multi-Model QuickStart](https://gettingstarted.intersystems.com/multimodel-overview/multimodel-quickstart/).
It shows object, relational, and native access from a .NET application to InterSystems IRIS. Airport data is stored using objects and retrieved using SQL, and a custom data structure is created using the Native API to handle route information between airports.

## Run the sample

In the integrated terminal, type: 
* `cd /home/project/quickstarts-multimodel-dotnet`
* `dotnet run`

## Output

If all works correctly, you will see a list of airports output. Data is stored using XEP (objects) and retrieved using ADO.net (relationally).  

If you would like to see how to store data natively using .NET:
1. Find and uncomment the following lines:   
`// storeAirfare(irisNative);`  
`// checkAirfare(irisNative);`
2. Enter departure airport: **BOS**
3. Enter destination airport: **AUS**

The output should say:  
>Printed to ^airport global. The distance in miles between BOS and AUS is: 1698.  
>The following routes exist for this path:  
>  -AA150: 450 USD  
>  -AA290: 550 USD  

Other routes may be null.

## Keep Exploring

To continue with another .NET example with InterSystems IRIS, see the [.NET QuickStart](https://gettingstarted.intersystems.com/language-quickstarts/net-quickstart/)
