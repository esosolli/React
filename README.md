
 import React, { useState, useEffect } from 'react';

function DataFetcher () {
    const[records,setRecords]=useState([])

    useEffect(() =>{
        const response= await fetch ("https://jsonplaceholder.typicode.com/users")
        .then(response => response.json())
        .then(data=> setRecords(data))
        .catch(err=> console.log (err))
    },
if (! data.length) return <div> Loading...</div>
    return ( 
        <div>
            <ul>
              <li> Name:{data[0].name}</li>
               <li> Email:{data[0]. Email il}</li>
               <li> Phone:{data[0].phone}</li>
                <li>Address:{data[0].address.street}</li>
            </ul>
        </div>
         );
        }
  
export default DataFetcher;