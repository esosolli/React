
 import React, { useState, useEffect } from 'react';

function FetchData() {
    const[records,setRecords]=useState([])

    useEffect(() => {
fetch("https://jsonplaceholder.typicode.com/users")
        .then(response => response.json())
        .then(data=> setRecords(data))
        .catch(err=> console.log (err))
    },)
if (!data.length ) return <div> Loading...</div>

return (
    
        <div>
            <ul>
              <li> Full name</li>
               <li> Email address</li>
               <li> Phone Number</li>
                <li>Address</li>
            </ul>
        </div>
         );
        }
export default FetchData;