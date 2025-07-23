
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
              <li> Name:{[Full name]}</li>
               <li> Email:{[email address]}</li>
               <li> Phone:{[phone number]}</li>
                <li>Address:{[Enter your address]}</li>
            </ul>
        </div>
         );
        }
  
export default DataFetcher;