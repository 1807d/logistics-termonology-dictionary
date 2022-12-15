
<!DOCTYPE html>
<html>

  <head>
    <title>Logistics and Shipping Terminology App</title>
  </head>

  <body>
    <h1>Logistics and Shipping Terminology App</h1>
    <p>Enter a term in the search bar below to view its definition:</p>
    <form>
      <input type="text" id="search-term">
      <input type="button" value="Search" onclick="lookupTerm()">
    </form>
    <p id="definition"></p>

    <script>
      // create a dictionary of terms and their definitions
      var logisticsDictionary = {
          "Logistics": "The process of planning, coordinating, and managing the movement of goods, services, and information from a source to a destination.",
          "Shipping": "The transport of goods and materials by sea, air, or land.",
          "Freight": "The goods or materials being transported by a shipping company.",
          "Forwarder": "A company that specializes in arranging the transportation of goods on behalf of its clients.",
          "Consignee": "The person or company to whom goods are shipped.",
          "Bill of lading": "A document that serves as a contract between the shipper and the carrier, detailing the type, quantity, and destination of the goods being transported." < script >
            // create a dictionary of terms and their definitions
            var logisticsDictionary = {
              "Logistics": "The process of planning, coordinating, and managing the movement of goods, services, and information from a source to a destination.",
              "Shipping": "The transport of goods and materials by sea, air, or land.",
              "Freight": "The goods or materials being transported by a shipping company.",
              "Forwarder": "A company that specializes in arranging the transportation of goods on behalf of its clients.",
              "Consignee": "The person or company to whom goods are shipped.",
              "Bill of lading": "A document that serves as a contract between the shipper and the carrier, detailing the type, quantity, and destination of the goods being transported.",
              "Carrier": "A company or individual that transports goods and materials.",
              "Shipper": "The person or company that contracts with a carrier to transport goods.",
              "Supply chain": "The network of organizations, people, activities, information, and resources involved in the production, handling, and distribution of goods and services.",
              "Transportation": "The movement of goods and materials from one location to another.",
              "Warehouse": "A commercial building for storage of goods and materials.",
              "Inventory": "The goods and materials held in stock by a business.",
              "Loading": "The act of placing goods and materials onto a vehicle or container for transport.",
              "Unloading": "The act of removing goods and materials from a vehicle or container after transport.",
              "Cross-docking": "The practice of transferring goods and materials directly from inbound vehicles or containers to outbound vehicles or containers, without intermediate storage or handling.",
              "Distribution center": "A facility used for the consolidation and distribution of goods and materials to multiple destinations.",
              "Stockpile": "A large quantity of goods and materials stored in one place.",
              "Stockroom": "A room or area used for storing goods and materials.",
              "Order fulfillment": "The process of completing customer orders and delivering the goods and materials to the customer.",
              "Pick and pack": "The process of selecting individual items from inventory and packing them for shipment to the customer.",
              "Dispatch": "The process of sending goods and materials to their destination.",
              "Routing": "The process of planning and organizing the movement of goods and materials from one location to another.",
              "Scheduling": "The process of planning and coordinating the timing of transportation and logistics activities.",
              "Tracking": "The process of monitoring the movement and status of goods and materials during transportation.",
              "Clearance": "The process of obtaining permission to enter or leave
            }

          // define a function to look up a term and display its definition on the page
          function lookupTerm() {
            // get the input term from the search bar
            var searchTerm = document.getElementById("search-term").value;

            // check if the term is in the dictionary
            if (searchTerm in logisticsDictionary) {
              // if it is, display the corresponding definition on the page
              document.getElementById("definition").innerHTML = logisticsDictionary[searchTerm];
            } else {
              // if it isn't, display an error message on the page
              document.getElementById("definition").innerHTML = "Sorry, that term is not in the dictionary.";
            }
          }

    </script>
  </body>

</html>
