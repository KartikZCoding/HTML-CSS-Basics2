# Create Simple Webpage using HTML & CSS

### Here's Wireframe of WebPage
![Second Web Development.png](https://github.com/KartikZCoding/HTML-CSS-Basics2/blob/a6debb65ee0949469cba7565ee84d78879a10868/My%20Second%20Web%20Page.png)

### HTML Code
```HTML
<!DOCTYPE html>
<html>

<head>
    <title>JOb's OP</title>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link
        href="https://fonts.googleapis.com/css2?family=Inter:wght@100..900&family=Roboto:ital,wght@0,400;0,500;0,700;0,900;1,400&display=swap"
        rel="stylesheet">
    <link rel="icon" href="./Images/job-logo.png" type="image/x-icon">
    <link rel="stylesheet" href="style.css">
</head>

<body>
    <!-- Header -->
    <header>
        <div id="navbar">
            <img src="./Images/job-logo.png" alt="logo" height="40px">
            <span id="logo-name">Job's Op</span>
        </div>
    </header>

    <!-- Banner Image -->
    <div id="banner-image">
        <img id="banner" src="./Images/banner.jpg" alt="Banner Image" height="360">
    </div>

    <!-- About -->
    <h1 id="about-head">
        About Job's
    </h1>
    <div id="about">
        <div id="description">
            <p style="margin-top: 0;">
                Jobs are evolving with technology and globalization, creating diverseopportunities in remote work, gig
                economy, and automation. Continuous learning, inclusivity, and jobsatisfaction are crucial for thriving
                in the dynamic labor market. Adaptability is key.</p>
            <p>
                We also offer 2 industry-focused bootcamp:
            <ol>
                <li>
                    <a target="_blank" href="#">FullStack Developer Bootcamp</a>
                </li>
                <li>
                    <a target="_blank" href="#">Data Science Bootcamp</a>
                </li>
            </ol>
            </p>
        </div>
        <div id="team">
            <img id="team-image" src="./Images/team.jpg" alt="Team Working Image">
        </div>
    </div>

    <!-- Jobs Opportunities -->
    <h2>Job Opportunities</h2>
    <div id="jobs">
        <table id="jobs-table">
            <tr class="jobs-header-row">
                <th rowspan="2">Job Title</th>
                <th colspan="2">Location</th>
                <th rowspan="2">Salary</th>
                <th rowspan="2">Posted On</th>
            </tr>
            <tr class="jobs-header-row">
                <th>City</th>
                <th>Coutry</th>
            </tr>
            <tr class="jobs-data-row">
                <td>Frontend Develoer</td>
                <td>Bengaluru</td>
                <td>India</td>
                <td>₹12,00,000</td>
                <td>Mar 3, 2023</td>
            </tr>
            <tr class="jobs-data-row">
                <td>Full Stack Developer</td>
                <td>New Delhi</td>
                <td>India</td>
                <td>₹15,00,000</td>
                <td>Feb 1, 2023</td>
            </tr>
            <tr class="jobs-data-row">
                <td>Data Scientist</td>
                <td>San Francisco</td>
                <td>USA</td>
                <td>$175,000</td>
                <td>Dec 22, 2022</td>
            </tr>
            <tr class="jobs-data-row">
                <td>ML Engineer</td>
                <td colspan="2">Remote</td>
                <td>$80,000</td>
                <td>Sep 19, 2022</td>
            </tr>
        </table>
    </div>

    <div id="application">
        <h2>Sumbit Your Application</h2>

        <form id="application-form" action="https://formbold.com/s/oJn7B" method="POST" enctype="multipart/form-data">
            <div class="form-group">
                <label for="name">Name</label><br>
                <input type="text" name="name" id="name" placeholder="Domjoi">
            </div>

            <div class="form-group">
                <label for="email">Email</label><br>
                <input type="tel" name="email" id="email" placeholder="abcd@gmail.com">
            </div>

            <div class="form-group">
                <label for="phone">Phone</label><br>
                <input type="number" name="phone" id="phone" placeholder="+918060583476">
            </div>

            <div class="form-group">
                <label for="dob">Date</label><br>
                <input type="date" name="dob" id="dob">
            </div>

            <div class="form-group">
                <label for="position">Position Applied</label><br>
                <select name="Position Applied" id="position">
                    <option value="">Select Position</option>
                    <option value="frontend">Frontend Developer</option>
                    <option value="fullstack">Full Stack Developer</option>
                    <option value="datascience">Data Science</option>
                    <option value="mlengineer">Ml Engineer</option>
                </select>
            </div>

            <div class="form-group">
                <label for="resume">Resume</label><br>
                <input type="file" name="resume" id="resume" accept=".pdf,.doc,.docx">
            </div>

            <div class="form-group">
                <label for="coverlatter">Cover Latter</label><br>
                <textarea name="coverlatter" id="coverlatter" rows="5"
                    placeholder="Explain what make you suitable for the job.."></textarea>
            </div>

            <div class="form-group">
                <label for="terms">
                    <input type="checkbox" name="terms" id="terms"> I agree to the terms and conditions
                </label>
            </div>

            <div class="form-group">
                <input type="submit" name="" id="" value="Submit">
            </div>
        </form>
    </div>

    <!-- Footer -->
    <div id="footer">
        <ul id="footer-links">
            <li>
                <a target="_blank" href="#">Cources</a>
            </li>
            <li>
                <a target="_blank" href="#">Programs</a>
            </li>
            <li>
                <a target="_blank" href="#">Youtube</a>
            </li>
        </ul>
        <span id="copyright">© 2024, Job's Op</span>
    </div>

</body>

</html>
```
### CSS Code
```CSS
html{
  font-size: 16px;
}

body {
  margin: 0;
  padding: 0;
  font-family: 'Roboto', sans-serif;
  font-size: 1rem;
  color: #444444;
}

h1, h2, h3, h4, h5, h6 {
  font-family: 'Inter', sans-serif;
  color: #222222;
}

a {
  text-decoration: none;
  color: #3b82f6;
}

a:hover {
  color: #1D4ED8;
}

/* Header */
#navbar {
  display: flex;
  align-items: center;
  max-width: 900px;
  margin: 5px auto;
  gap: 8px;
}
#logo-name {
  font-weight: bold;
  font-family: "Franklin Gothic Medium", "Arial Narrow", Arial, sans-serif;
  font-size: 22px;
}

/* Banner Image */
#banner-image {
  max-width: 900px;
  margin: 0 auto;
}
#banner {
  width: 100%;
  object-fit: cover;
}

/* About */
#about-head {
  text-align: center;
}
#about {
  display: flex;
  max-width: 900px;
  margin: 0 auto;
  padding: 8px;
}
#description {
  width: 50%;
  padding-right: 8px;
}
#team {
  width: 50%;
}
#team-image {
  border-radius: 5px;
  width: 100%;
}

/* Job Opportunities */
h2 {
  text-align: center;
}
#jobs {
  max-width: 900px;
  margin: 0 auto;
  padding: 0 8px;
}
#jobs-table {
  width: 100%;
  border: 1px solid gray;
  border-collapse: collapse;
}
.jobs-header-row th{
  border: 1px solid gray;
  padding: 8px;
  background-color: #bae6fd;
  text-align: center;
  color: #222222;
}
.jobs-data-row td {
  border: 1px solid gray;
  padding: 8px;
}
#jobs-table tr:nth-child(odd) {
  background-color: #e0f2fe;
}

/* Form */
#application {
  max-width: 900px;
  margin: 0 auto;
  padding: 0 8px;
}

#application h2 {
  margin-top: 35px;
}

.form-group {
  margin: 16px;
}

#application-form label {
  font-weight: 600;
  font-size: 1.15rem;
}

#application-form input,select,textarea {
  padding: 4px;
  font-size: 1.25rem;
  margin-top: 4px;
  border-radius: 5px;
  border: 1px solid gray;
}

.form-group textarea {
  width: 60%;
  font-family: 'Roboto', sans-serif;
}

.form-group input[type="checkbox"] {
  width: 16px;
  height: 16px;
}

.form-group input[type="submit"] {
  background-color: #3b82f6;
  color: white;
  font-weight: 500;
  padding: 26px;
  cursor: pointer;
}

/* Footer */
#footer {
  background-color: ghostwhite;
  padding: 8px;
  padding-bottom: 20px;
  margin-top: 35px;
  text-align: center;
}
#footer-links {
  list-style: none;
}
#footer-links li {
  display: inline-block;
  margin: 0 16px;
}
#copyright {
  color: #6b7280;
}
```
### Here's all Images
<a href="https://github.com/KartikZCoding/HTML-CSS-Basics2/tree/7577f8cde026444e849a2d8cc1e70bcd0aef1853/src/Images">
    <img src="https://github.com/KartikZCoding/Other-Files/blob/29c62f9aa8abe0470d9e2d75c809940a786cf035/image-logo.png" alt="Image Icon" height="90px">
</a>
