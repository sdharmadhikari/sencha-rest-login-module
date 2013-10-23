sencha-rest-login-module
========================


Login Module For Sencha Touch.

Pluggable Login Component for Sencha Touch.
* All handlers are inside the component and not in controllers. This has been done to make sure component is pluggable easily in other Sencha Touch Projects.
* Application wide event is triggered so that it can be captured anywhere. For example event "signInSuccess" event is fired application wide.

Currently supports Sencha Touch 2.2.1
The module is developed using Sencha Architect. Contributors are expected to use sencha architect possibly because metadata of SA can be in sync with code.

Uses sencha-roo-backend as sample backend. 

* HTTPS communication is assumed.
* Password is Base64 encoded. 
* "Snap Sign Up" button should push "Sencha Signup Module" which is separate Github project.
* Component has loginUrl attribute which can be customized as needed.
* userObject received from server passed along with signInSuccess event so that main project can use it.
* Currently plain password is part of userObject, it can be used to send credentials every time in case of stateless (REST) based server. Client side encryption of plain password will be in future.
