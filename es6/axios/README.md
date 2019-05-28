 # axios API interaction
 
 ## You will need to import axios for use
 
#### Post call for data to be stored in DB
     ```javascript
     const newUser = {
                name,
                email,
                password
            }

            try {
                // Make header for post
                const config = {
                    headers: {
                        'Content-Type': 'application/json'
                    }
                }

                // prepare body in string
                const body = JSON.stringify(newUser);

                // Use post method to interact with api usin axios
                const res = await axios.post('/api/users', body, config);

                console.log(res.data);

            } catch (err) {
                console.error(err.response.data);
            }
            ```javascript
