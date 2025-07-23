
 import React, { useState, useEffect } from 'react';

function DataFetcher () {
    const[records,setRecords]=useState([])

    useEffect(() => {
fetch("https://jsonplaceholder.typicode.com/users")
        .then(response => response.json())
        .then(data=> setRecords(data))
        .catch(err=> console.log (err))
    },)
if (! data.length) return <div> Loading...</div>
    
        <div>
            <ul>
              <li> Name:{[ Enter your name]}</li>
               <li> Email:{[Enter your email address]}</li>
               <li> Phone:{[Enter your phone number]}</li>
                <li>Address:{[Enter your address]}</li>
            </ul>
        </div>
         );
        }
  
export default DataFetcher;