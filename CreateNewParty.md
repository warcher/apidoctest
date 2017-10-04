**Create new party**
----
  Returns json data about a single user.

* **URL**

  /api/party

* **Method:**

  `POST`
  
*  **URL Params**

   **Required:**
 
   `id=[integer]`

* **Data Params**

  None

* **Success Response:**

  * **Code:** 200 <br />
    **Content:** `{ id : 12, name : "Michael Bloom" }`
 
* **Error Response:**

  * **Code:** 404 NOT FOUND <br />
    **Content:** `{ error : "User doesn't exist" }`

  OR

  * **Code:** 401 UNAUTHORIZED <br />
    **Content:** `{ error : "You are unauthorized to make this request." }`

* **Body:**

`{
   "$type": "Asi.Soa.Membership.DataContracts.PersonData, Asi.Soa.Membership.Contracts",
   "PersonName": {
                "$type": "Asi.Soa.Membership.DataContracts.PersonNameData, Asi.Soa.Membership.Contracts",
                "FirstName": "George",
                "InformalName": "Gee",
                "LastName": "Smith",
                "NamePrefix": "Mr."               
            }
}`
