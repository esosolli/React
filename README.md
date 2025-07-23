
 import React, { useState, useEffect } from 'react';

function DataFetcher () {
    const[records,setRecords]=useState([])

useEffect(() => {"\n const fetchData = async () => {\n try {\n const response = await fetch(\"https://jsonplaceholder.typicode.com/users\");\n          
const data = await response.json();\n               setRecords(data);\n"}
 catch (err) {"\n console.log(err);\n"}
  };
  fetchData();
}, []);


if (! data.length) return <div> Loading...</div>
    return ( 
        <div>
            <ul>
              <li> Name:{data[0].name}</li>
               <li> Email:{data[0]. Email}</li>
               <li> Phone:{data[0].phone}</li>
                <li>Address:{data[0].address.street}</li>
            </ul>
        </div>
         );
        }
  
export default DataFetcher;