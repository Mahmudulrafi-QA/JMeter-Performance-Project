# 🌐 JMeter Performance Testing Project

This repository contains a complete JMeter project for performance testing of a sample e-commerce website. It includes multiple components like Aggregate Graph, HTTP Header Manager, User Defined Variables, and more, to simulate real-world user behavior and analyze system performance.

---

## 🚀 Project Overview

This JMeter Test Plan is designed to:
- Simulate multiple users browsing different product categories.
- Validate API responses and server performance.
- Generate detailed reports using listeners like **Aggregate Graph** and **Response Time Graph**.

---

## 📦 Project Structure

JMeter-Performance-Project/
│
├── TestPlan.jmx # Main JMeter test plan
├── README.md # Project documentation

## ⚙️ Test Plan Components

The test plan includes:

✅ **Thread Group**
- Simulates multiple concurrent users
- Configured with Ramp-Up Period and Loop Count

✅ **Config Elements**
- **HTTP Header Manager**: Adds necessary HTTP headers
- **User Defined Variables**: Stores reusable variables
- **HTTP Request Defaults**: Default server name and protocol
- **DNS Cache Manager**: Manages DNS caching
- **HTTP Authorization Manager**: Handles authentication
- **HTTP Cookie Manager**: Manages cookies
- **HTTP Cache Manager**: Simulates browser caching

✅ **Samplers**
- **Browser Category Home Page**: Loads the home page
- **Browse Phone Category**: Simulates browsing phone category

✅ **Listeners**
- **Aggregate Graph**: Displays summary of performance metrics
- **Response Time Graph**: Shows response time trends
- **View Results Tree**: Debugging and viewing detailed responses

---

## 📊 Reports

After running the test, you can analyze performance using:
- **Aggregate Report**
- **Response Time Graph**
- **HTML Report (Auto-generated)**

---

## 🔥 How to Run

1. Open Apache JMeter
2. Load `TestPlan.jmx`
3. Configure the number of threads, ramp-up period, and loop count as needed
4. Click ▶️ Start to run the test
5. View results in Listeners or generate an HTML report:
    ```bash
    jmeter -n -t TestPlan.jmx -l results.jtl -e -o Reports/
    ```

---

## 📌 Tools & Technologies
- [Apache JMeter 5.x](https://jmeter.apache.org/)
- Java JDK 8 or higher
- GitHub for version control

---

## 📈 Sample Results
| Metric               | Value     |
|---------------------|-----------|
| Average Response Time| 350 ms    |
| Throughput           | 500 req/sec|
| Error Rate           | 0.5%      |

---

## 👨‍💻 Author
Mahmudul Hasan Rafi  
💼 SQA Engineer | Performance Tester  
email:mahmudulrafi1998@gmail.com

---

## 📂 License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
