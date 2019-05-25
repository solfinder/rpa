# rpa
Robotic Process Automation

Steps for execution:
-------------------
1) Start apache server on test machine.Extract ShippingBill.zip into htdocs/shippingbill folder of running apache server. Verify that http://localhost:8080/shippingbill/shippingbill.html is accessible.
[Note if the url is different you will need to make the update to SBGenerator.xaml accordingly]
2) Open the ExprterAssist project in UIPath.
3) Excel file sb.xlsx contains the test data for generation of shipping bills. You can add more rows to rows file but you will need to update the excel read range activity accordingly.
4) Run the SBGenerator.xaml sequence from UIPath.
5) On successful run you will have shipping bills generated in EDI format as <billindex>.sb files . These files contain electronic shipping bills which can be uploaded to customs department websote for export cleranace.
6) Two sample bills 0.sb and 1.sb are uploaded for reference.

Video: https://youtu.be/0j-JTfZlXw4
