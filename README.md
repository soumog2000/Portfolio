.App {
  text-align: center;
}

.App-logo {
  height: 40vmin;
  pointer-events: none;
}

@media (prefers-reduced-motion: no-preference) {
  .App-logo {
    animation: App-logo-spin infinite 20s linear;
  }
}

.App-header {
  background-color: #282c34;
  min-height: 100vh;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  font-size: calc(10px + 2vmin);
  color: white;
}

.App-link {
  color: #61dafb;
}

@keyframes App-logo-spin {
  from {
    transform: rotate(0deg);
  }
  to {
    transform: rotate(360deg);
  }
}
.container-fluid{
  color:black
}
h2{
padding:15px 15px 15px 15px
}
.head{
    padding: 5px; 
    border: 2px solid black;  
} 
.home{
  text-decoration: none;
  padding:12px
}
.h2{
  padding:10px
}

.welcome{
  font-size: 20px;
  padding-left: 10px;
  text-decoration: none;
  color:blue
  
}
.welcome:hover{
  color:red
}
.button{
  color:purple;
  border:2px solid purple;
  padding-right:10px;
  padding-top: 9px;
  font-size: 15px;
}
.button1{
  color:purple;
  border:2px solid purple;
  padding-top: 9px;
  font-size: 15px;
}
.btn1{
  border:1px solid black;
  border-radius: 10px;
  margin:10px
}

.table{
  border: 1px solid black;
}
.tr{
  border:1px solid black
}
.th{
  border:1px solid black;
}
.td{
  border:1px solid black;
 
}
.td1{
  border:1px solid black;
  height:20vh;
}
.lab{
   display: flex;
}
.opt{
display: flex;
width:186px;
margin-left: 13px;
}
.btn12{
  border:1px solid black;
  border-radius: 10px;
  margin:10px;
  padding-left: 25px;
  padding-right: 25px;
}
.right{
  display: flex;
  text-align: right;
  font-size: 20px;
}
.left{
  display: flex;
  font-size: 20px;
  float: right;
}
.left1{
  display: flex;
  font-size: 20px;
  float: right;
}
.in{
  width: 187px;
  height: 30px;
  margin-left: 48px;
  margin-top: 22px;
}
.lab1{
  margin-top: 22px;
}


*******************************************************************************


import React from "react";

export default class Viewsavedreport extends React.Component {
    render() {
        return (
            <div className="head container-fluid">
                <div className="container-fluid">
                    <h2 className="text-center bg-warning">Performance Management System</h2>
                </div>
                <div className="row">
                    <div className="col-md-9">
                    <p className='welcome'>Welcome View</p>
                    </div>
                <div className="col-md-3">
                <button className='btn btn-info'>Change Password</button>&nbsp;&nbsp;
                    <button className='btn btn-danger'>Logout</button>

                    </div>
                </div>
              
                <nav className="navbar navbar-expand-lg bg-body-tertiary">
  <div className="container-fluid nav-tabs">
      <button className="btn btn-outline-primary">Home</button>&nbsp;
    
    <button className="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
      <span className="navbar-toggler-icon"></span>
    </button>
    <div className="collapse navbar-collapse" id="navbarSupportedContent">
      <ul className="navbar-nav me-auto mb-2 mb-lg-0">
        <li className="nav-item">
        <button className="btn btn-outline-primary" type="submit">View Saved Report</button>
        </li>
</ul>
</div>
</div>
</nav><br/>

                <div className="row">
                    <div className="left col-md-6">
                        <h5><lable className="lab">Device Name</lable></h5>
                        <select className="opt">
                            <option>-------Select--------</option>
                            <option>Router</option>
                        </select>
                    </div>
                    <div className="right col-md-6">
                    <h5><lable className="lab">Saved Report</lable></h5>
                        <select className="opt">
                            <option>-------Select--------</option>
                            <option>Report_18Jan</option>
                        </select>
                    </div>
                </div>
               
                <div className="row">
                    <div className="col-md-12 left1">
                    <h5 className="lab1">Device IP</h5>
                    <input type="text" className="in"/>
                    </div>

                </div>
                <div className="row">
                    <div className="col-md-6">
                    </div>
                <div className='buttona col-md-6'>
                    <button className='btn12'>View</button>
                    <button className='btn1'>Generate Chart</button>
                </div>
                </div>
                <div>
                    <table className='table table-bordered border-black text-center'>
                        <thead>
                            <tr className='tr' style={{ border: "1px solid black" }}>
                                <th rowSpan={"2"}>Date & Time</th>
                                <th rowSpan={"2"}>Availability</th>
                                <th rowSpan={"2"}>Interface Status</th>
                                <th colSpan={"3"}>Utilization</th>
                            </tr>
                            <tr className='tr'>
                                <th>CPU</th>
                                <th>Memory</th>
                                <th>Disk</th>
                            </tr>

                            <tr className='td' >
                                <th rowSpan={"2"}></th>
                                <th rowSpan={"2"}></th>
                                <th rowSpan={"2"}></th>

                            </tr>
                            <tr className='td1 td'>
                                <th rowSpan={"2"} ></th>
                                <th rowSpan={"2"}></th>
                                <th rowSpan={"2"}></th>
                            </tr>
                        </thead>
                    </table>
                </div>
            </div>
        )

    }
}
