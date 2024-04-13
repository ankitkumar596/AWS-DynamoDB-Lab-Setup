# AWS DynamoDB Practice Lab

## Steps

### Step 1: Search DynamoDB

1. In the top navigation bar search box, type: `dynamodb`.
2. In the search results, under Services, click **DynamoDB**.
3. Go to the next step.

    ![alt text](<Screenshot from 2024-04-13 06-57-10.png>)

---

### Step 2: Create DynamoDB Table

1. On the Amazon DynamoDB console home page, click **Create table**.
2. Go to the next step.

    ![alt text](<Screenshot from 2024-04-13 06-57-44.png>)

----

### Step 3: Table Details

1. In the **Table details** section, for **Table name**, type: `UserVideoHistory`.
2. For **Partition key**, in the left text box, type: `userId`.
   - You must type the partition key exactly as shown, userId with an uppercase I because keys are case sensitive.
3. On the right dropdown menu, choose **String**.
4. For **Sort key**, in the left text box, type: `lastDateWatched`.
5. On the right dropdown menu, choose **Number**.
6. Scroll down to the bottom of the page.
7. Go to the next step.

    ![alt text](<Screenshot from 2024-04-13 07-00-31.png>)

---

### Step 4: Settings

1. In the **Settings** section, keep the default settings.
2. Click **Create table**.
3. Go to the next step.

---

### Step 5: Review Table Status

1. In the **Tables** section, under **Status**, review the status of the table.
   - Wait for the status to change to **Active**.
2. When active, click the table name.
3. Go to the next step.

    ![alt text](<Screenshot from 2024-04-13 07-02-53.png>)
    ![alt text](<Screenshot from 2024-04-13 07-03-26.png>)

---

### Step 6: Create Item

1. Click **Actions** to expand the dropdown menu.
2. Choose **Create item**.
3. Go to the next step.

    ![alt text](<Screenshot from 2024-04-13 07-04-38.png>)

---

### Step 7: Add Attributes

1. In the **Attributes** section, next to **userId**, for **Value**, type: `12345-abcd-6789`.
2. Next to **lastDateWatched**, for **Value**, type: `1619156406`.
   - This is a UNIX timestamp.
3. Go to the next step.

    ![alt text](<Screenshot from 2024-04-13 07-06-47.png>)

---

### Step 8: Add Additional Attributes

1. To add another attribute, click **Add new attribute** to expand the dropdown menu.
2. Choose **String**.
3. Go to the next step.


---

### Step 9: Define Attribute "videoId"

1. For **Attribute name**, in the new text box, type: `videoId`.
2. For **Value**, in the new text box, type: `9875-djac-1859`.
3. Go to the next step.

    ![alt text](<Screenshot from 2024-04-13 07-10-05-1.png>)

---

### Step 10: Add Another Attribute

1. Click **Add new attribute**.
2. Choose **String**.
3. Go to the next step.


---

### Step 11: Define Attribute "preferredLanguage"

1. For **Attribute name**, type: `preferredLanguage`.
2. For **Value**, type: `English`.
3. Go to the next step.

    ![alt text](<Screenshot from 2024-04-13 07-10-34-1.png>)
---

### Step 12: Add a List Attribute

1. Click **Add new attribute**.
2. Choose **List**.
3. Go to the next step.

---

### Step 13: Define Attribute "supportedDeviceTypes"

1. For **Attribute name**, type: `supportedDeviceTypes`.
2. Go to the next step.

    ![alt text](<Screenshot from 2024-04-13 07-11-52.png>)
---

### Step 14: Add Values to List Attribute

1. For **Value**, click **Insert a field** to expand the dropdown menu.
2. Choose **String**.
3. Go to the next step.

---

### Step 15: Add Supported Device Types

1. For **Attribute name**, next to **supportDeviceTypes**, click the plus sign (+).
2. For **Value**, in the new text box, type: `Amazon Fire TV`.
3. Go to the next step.

    ![alt text](<Screenshot from 2024-04-13 07-12-27.png>)
---

### Step 16: Add Another Value

1. For **Value**, click **Insert a field**.
2. Choose **String**.
3. Go to the next step.

    ![alt text](<Screenshot from 2024-04-13 07-12-52.png>)
---

### Step 17: Add Second Device Type

1. For **Value**, in the new text box, type: `Amazon Fire Tablet`.
2. Click **Create item**.
3. Go to the next step.

---

### Step 18: Explore Items

1. In the left navigation pane, under **Tables**, click **Explore items**.
2. In the **Items returned** section, under **userId**, click **12345-abcd-6789**.

    ![alt text](<Screenshot from 2024-04-13 07-14-59.png>)

   - You can now edit the record again.
3. Go to the next step.
    
---

### Step 19: Add Another Attribute

1. Click **Add new attribute**.
2. Choose **Number**.
3. Go to the next step.

---

### Step 20: Define Attribute "lastStopTime"

1. For **Attribute name**, type: `lastStopTime`.
2. For **Value**, type: `90`.
3. Click **Save and close**.
4. Go to the next step.

    ![alt text](<Screenshot from 2024-04-13 07-15-52.png>)

---

### Step 21: Query Items

1. To expand the section, click **Scan/Query items**.
2. Click the **Query** tab.
3. For **userId (Partition key)**, type: `12345-abcd-6789`.
4. For **lastDateWatch (Sort Key)**, on the left dropdown menu, choose **Greater than**.
5. In the right text box, type: `1609477200`.
6. Click **Run**.
7. Go to the next step.

    ![alt text](<Screenshot from 2024-04-13 07-17-23.png>)
---

### Step 22: Review Query Results

1. In the **Items returned** section, review the returned record.
2. Go to the next step.

    ![alt text](<Screenshot from 2024-04-13 07-17-58.png>)

---

### Step 23: Change Query Criteria

1. To change the query criteria, for **userId**, type: `abd5-zxcg-12385`.
2. Click **Run**.
3. In the **Items returned** section, review the results.
   - Nothing is returned because no record matches the partition key and has a sort key greater than what has been entered.
4. Go to the next step.

    ![alt text](<Screenshot from 2024-04-13 07-19-11.png>)

    ![alt text](<Screenshot from 2024-04-13 07-19-20.png>)

---

### Step 24: Scan Items

1. Click the **Scan** tab.
2. Click **Run**.
3. In the **Items returned** section, review the results.
   - All items in your DynamoDB table should be listed.
4. Go to the next step.

    ![alt text](<Screenshot from 2024-04-13 07-19-56.png>)
---

## Congratulations!

You've completed the Practice section. Go to the DIY section to complete the solution.

---

Feel free to adjust formatting as needed!
