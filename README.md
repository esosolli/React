
 import React, { useState, useEffect } from 'react';

function DataFetcher () {
    const[records,setRecords]=useState([])

    useEffect(() =>{
        const response=>`await fetch` ("https://jsonplaceholder.typicode.com/users")
        .then(response => response.json())
        .then(data=> setRecords(data))
        .catch(err=> console.log (err))
    },
if (! data.length) return <div> Loading...</div>
    return ( 
        <div>
            <ul>
              <li> Name:{Full name].name}</li>
               <li> Email:{email address]. Email}</li>
               <li> Phone:{phone number].phone}</li>
                <li>Address:{data[0].address.street}</li>
            </ul>
        </div>
         );
        }
  
export default DataFetcher;