# How to use ASPxUploadControl in the Edit Appointment Form


<p>This example demonstrates how to use <a href="https://documentation.devexpress.com/#AspNet/clsDevExpressWebASPxUploadControlASPxUploadControltopic">ASPxUploadControl</a> inside a custom <strong>Appointment</strong> <strong>Editing</strong> <strong>Form</strong> to load an image to a custom appointment field.</p>
<p>To accomplish this task, perform the following steps:</p>
<p>1. Create a custom <strong>Appointment</strong> <strong>Editing</strong> <strong>Form</strong>.<br />2. Create a custom <a href="https://documentation.devexpress.com/#WPF/clsDevExpressXpfSchedulerUIAppointmentFormControllertopic">AppointmentFormController</a> class with corresponding additional properties for each custom field.<br />3. Override the <strong>AppointmentFormSaveCallback</strong> command to pass custom editor values to the mentioned <strong>AppointmentFormController</strong> properties.<br />4. Put the <strong>ASPxUploadControl </strong>onto a custom<strong> Appointment Editing Form.<br /></strong>5. Handle the <a href="http://documentation.devexpress.com/#AspNet/DevExpressWebASPxUploadControlASPxUploadControl_FileUploadCompletetopic">ASPxUploadControl.FileUploadComplete</a> event. <br /><br />When an end-user have uploaded a file, the <strong>ASPxUploadControl.FileUploadComplete</strong> event is raised.</p>
<p>In this event handler, an uploaded file name (string) or uploaded file content (byte array) are obtain and save the required parameter in the appointment's source object. </p>
<p>The custom form contains the <a href="https://documentation.devexpress.com/#AspNet/clsDevExpressWebASPxEditorsASPxImagetopic">ASPxImage</a> control which shows the uploaded image.</p>

<br/>

