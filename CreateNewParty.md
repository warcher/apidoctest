**Create new party**
----
  Returns json data about a single user.

* **URL**

  /api/party

* **Method:**

  <span style="background-color:orange;color:white">POST</span>
  
*  **URL Params**

   **Required:**
 
   None

* **Data Params**

  None

* **Success Response:**

  * **Code:** 200 <br />
 
* **Error Response:**

  * **Code:** 404 NOT FOUND <br />

  OR

  * **Code:** 401 UNAUTHORIZED <br />
    **Content:** `{ error : "You are unauthorized to make this request." }`

* **Body:**

```
{
   "$type": "Asi.Soa.Membership.DataContracts.PersonData, Asi.Soa.Membership.Contracts",
   "PersonName": {
                "$type": "Asi.Soa.Membership.DataContracts.PersonNameData, Asi.Soa.Membership.Contracts",
                "FirstName": "George",
                "InformalName": "Gee",
                "LastName": "Smith",
                "NamePrefix": "Mr."               
            },
}
```
