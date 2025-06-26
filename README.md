# Call-Center-Project


![e51bde380fa76884c12633236ba3ee10](https://github.com/user-attachments/assets/218cee63-1df6-44d4-b7af-425deb49d294)

# Task
Create a Power BI dashboard to help the Call Centre Manager track key performance metrics and short-term behavioural trends, supporting clearer, data-driven decisions.

The dashboard should show answered vs. abandoned calls, speed of answer, call duration, and how customer satisfaction is trending over time. It should also surface any patterns in customer or agent behaviour that may signal issues or areas for improvement.

The design must be intuitive, visually clear, and ready for management discussions, with a strong focus on highlighting trends and insights in a clean, presentation-friendly format.

# Process
In Power BI Editor, I performed the following data transformation steps:
promoted headers, changed the data types of relevant columns to their appropriate types (e.g., date, time, text, etc.) to enable accurate calculations and avoid errors. Also calculated call duration in seconds by:
1. Duplicatingthe time column (representing call duration).
2. Then converted the duplicated column to the Duration data type.
3. Next, I added a custom column using the formula:
Duration.TotalSeconds([DuplicatedColumn] - #time(0, 0, 0)).  

This formula calculates the total duration of each call in seconds by subtracting midnight (#time(0,0,0)) from the call time and converting the result to seconds.

<img width="1247" alt="image" src="https://github.com/user-attachments/assets/9861b3bd-d2be-4e6a-9035-ca11500ab58a" />

# Analyze

I have created measures to answer the questions and provide the following KPIs. Here are some of them:  
<br><br>

- ### Positive Satisfaction Rating  
  ![Positive Satisfaction Rating](https://github.com/user-attachments/assets/be40134b-9aab-4fed-85be-0fb5fa7f0caf)  
<br><br>

- ### Total Calls Abandoned  
  ![Total Calls Abandoned](https://github.com/user-attachments/assets/5b057c73-05d3-4fda-8c77-08bd25204793)  
<br><br>

- ### Total Calls Answered  
  ![Total Calls Answered](https://github.com/user-attachments/assets/e96d15d8-2839-40be-8811-c532cea5b4b6)  
<br><br>

- ### Overall Customer Satisfaction  
  ![Overall Customer Satisfaction](https://github.com/user-attachments/assets/8f04afce-a596-4f7c-a654-7d9a713f2e9e)  
<br><br>

- ### After getting all the required measures, I added cards in my dashboard to show all the KPIs at the top.  
  ![KPI Cards](https://github.com/user-attachments/assets/02a4daa9-3015-4c41-ac32-bcd7f3979422)  
<br><br>

- ### Average Talk Duration  
  Next, I created a bar chart to show the average talk duration of agents. Jim has the longest talk duration and Becky is the fastest.
  <br><br>
  ![Average Talk Duration](https://github.com/user-attachments/assets/798f2b8f-8f4b-4a2f-bb0b-5ac0b8fd75aa)  
<br><br>

- ### Resolved Calls Per Day  
  Then, I created a column chart that shows total resolved calls per day of the week. It shows that every Monday and Saturday, agents have higher resolved calls than the rest of the week.
  <br><br>
  ![Resolved Calls Per Day](https://github.com/user-attachments/assets/ef483d13-a9e1-4a4e-b34f-e54ee90ffa19)  
<br><br>

- ### Agent Stats Table  
  To summarize all the stats of the agents, I inserted a table that shows their total calls, answered calls, abandoned calls, resolved calls, unresolved calls, and satisfaction ratings.
  <br><br> 
  ![Agent Stats Table](https://github.com/user-attachments/assets/067c52da-b139-4808-abc6-b900586e57e0)  
<br><br>

- ### Call Topics Treemap  
  The last visualization is a treemap showing all the call topics.
  <br><br>
  ![Call Topics Treemap](https://github.com/user-attachments/assets/5a8daa1f-55af-4c32-bf63-41e9fc908fdc)  
<br><br>

- ### Final Dashboard  
  Finally, I designed the dashboard and created the background.
  <br><br>
  ![Final Dashboard](https://github.com/user-attachments/assets/b37853f7-7fc3-46c2-baf6-3ddd9bd1d6d4)  
<br><br>

---

## 📊 INSIGHTS

- The **call abandonment rate is 17.3%** (149 out of 862), indicating many customers hang up before reaching an agent—likely due to the **average answer time of 68.51 seconds**.
- **Customer satisfaction is low at 48.95%**, signaling issues with service quality or resolution effectiveness.
- **Greg and Joe** have strong performance metrics, with high resolved calls and above-average satisfaction.
- **Stewart and Becky** show lower satisfaction scores, suggesting a need for **training or support**.
- **Monday and Friday** show the most resolved calls, pointing to **peak demand** at the start and end of the week.
- **Top call topics** include **Payment-related issues** and **Technical Support**, highlighting key service areas.

---

## ✅ RECOMMENDATIONS

- **Reduce Abandoned Calls:**  
  Introduce a **callback option** and optimize staffing during peak periods, especially Mondays and Fridays.

- **Improve Response Time:**  
  Streamline call routing and consider **automated systems** for basic queries.

- **Boost Customer Satisfaction:**  
  Provide **coaching** for lower-performing agents and implement **real-time feedback surveys**.

- **Leverage Strong Performers:**  
  Use agents like **Greg and Joe as peer mentors** or best practice models.

- **Enhance Topic Handling:**  
  Assign agents by **topic expertise** and build **self-service resources** for common inquiries like payments and tech issues.

---













