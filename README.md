# graphqldemo
This example is for integrating GraphQL API along with the Spring Boot application. This application has two operatons. One is creating a new vehicle and the second one is querying the vehicles.

Creates a new vehicle:

mutation {
  createVehicle(type: "car", modelCode: "XYZ0193", brandName: "XYZ", launchDate: "2016-10-11") 
  {
    id
  }
}

List Vehicles:

query {
  vehicles(count: 10) 
  {
    id, 
    type, 
    modelCode
}
}
