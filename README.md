# Cypress-Learning
<ul>
<li>A frontend web automation testing tool<br></li>
<li>It is used for modern web application (like React Js, AngularJs....)<br></li>
<li>Using Cypress you can automate any application which runs on the browser.<br></li>
<li>Cypress use Javascript/Typescript for writing automated test cases.<br></li>
<li>It doesn't use any selenium library because it is totally different than selenium.<br></li>
<li>It is a open source.<br></li>
</ul>

Cypress has multiple components, like:
<ul>        
  <li>Test Runner which is Free to use and by using this we can install cypress and write our test cases and,<br></li>
  <li>Dashboard which is Paid which helps in maintain the test history and then parallel testing.</li>
</ul> 
<ul>
<li>It is totally build on Node.js environment and comes with npm module.</li> 
<li>We can automate End-to-End test cases.</li>
<li>Used for Integerated tests.</li>
<li>Used to perform Unit test cases.</li>
<li>Used for API testing</li>
</ul>
<br>
<table>
  <tr>
    <th></th>
    <th>Selenium</th>
    <th>Cypress</th>
  </tr>
  <tr>
    <td>Application Support</td>
    <td>Only Web</td>
    <td>Web & API</td>
  </tr>
  <tr>
    <td>Cost</td>
    <td>Free</td>
    <td>Test Runner - Free, Dashboard - Paid</td>
  </tr>
  <tr>
    <td>Setup & Installation</td>
    <td>Difficult</td>
    <td>Easier</td>
  </tr>
  <tr>
    <td>Languages</td>
    <td>Java, Python, Ruby, C#, JavaScript</td>
    <td>Javascript, Typescript</td>
  </tr>
  <tr>
    <td>Browsers</td>
    <td>Chrome, Edge, Firefox, Safari,<br> Opera & IE11</td>
    <td>Chrome, Edge, Firefox, & Electron</td>
  </tr>
  <tr>
    <td>Frameworks Support</td>
    <td>Junit, TestNG, pyTest etc. based on <br> programming language</td>
    <td>Mocha JS</td>
  </tr>
  <tr>
    <td>Performance</td>
    <td>Run Outside of the browser. So performance <br> is slow when compare with Cypress.</td>
    <td>Faster since it runs inside of the browser.</td>
  </tr>
  <tr>
    <td>Reporting</td>
    <td>Integerate with Extent, Allure etc...</td>
    <td>Mocha Reporters, Cypress Dashboard</td>
  </tr>
</table>
<br>

**Cypress Ecosystem**
<li>Test Runner ---- open source, locally installed</li>
<li>Dasborad ---- Paid</li>
<br>

**Features**
<li><b>Time travel --></b> that means cypress takes snapshot of every step which is running, <br>  Suppose if there are 10 lines of code the cypress will take every snap shot of the step and, <br>  Suppose you are on 5th line so now you can also go back to run the previous line or otherwise forward.</li><br>
<li><b>Debuggability --></b> Cypress have acces to all dev tools i.e while running a code if some error occurs you can debug the code there itself <br> without running the code once again.</li><br>
<li><b>Automatic Wait (Built-in Wait) --></b> that means if some element takes time to load or a page takes time to load without using any other function, it has this special feature which waits automatically for the element to get load and then perform the action.</li><br>
<li><b>Consistency --></b> Cypress provide consistent results because it runs inside the browser.</li><br>
<li><b>Screenshots & Videos --></b>When you run test cases if something got failed the screen shot will get automatically captured and same test  cases will be recorded in video format.</li><br>
<li><b>Cross Browser Testing --></b> that means it helps to run test cases on multiple browsers which are supported</li><br>
<br>

**Limitations**
<li>We can't automate windows based or mobile applications.</li>
<li>Limited support of browsers.</li>
<li>Suports only Javascript/Typescript.</li>
<li>Reading writing data into files are difficult.</li>
<li>Third Party reporting tool integration is also limited.</li>

**Environment Setup**
<ol>
  <li>Download and install Node.js</li>
  <li>Download and install vidual studio code (vscode)</li>
  <li>Crete a new folder for project and open in vscode</li>
  <li>open cmd/terminal then execute below command </li>
  &emsp;   <b>npm -i init    ----> creates a package.json file</b>
  <li>To install cypress</li>
  &emsp;  <b>npm install cypress --save -dev</b>
  <li>Start cypress</li>
  &emsp;  <b>npx cypress open</b> &emsp;  (or)<br>
  &emsp;  <b>node_modules/.bin/cypress open</b>
</ol>

**Writting & Executing Tests**

        describe('Suite Name', () => {
        
          it('Test1', () => {
            expect(true).to.equal(true)
          })

          it('Test2', () => {
            expect(true).to.equal(true)
          })          
        })

        (or)

        describe('Suite Name', function()
        {
          it('Test1', () => {
            expect(true).to.equal(true)
          })

          it('Test2', () => {
            expect(true).to.equal(true)
          })
        }
        )
