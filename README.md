# PCF-Services

i) Npcf_AMPolicyControl

It provides AMF with policy information about the UE or provides the access and mobility related policy information to the UE. In addition, it also provide access selection policy, which dictates that which radio access technology should get priority in a given context. It also have different service operation such as 
	
- Create: creates association of AMF and PCF for a particular device.

- Update: When that association receives an update it was handled here turn. 

- Notify: It can be used by PCF when there is no request from the AMF. At anytime PCF use this to update policies in AMF.

- Delete: To delete the association corresponding to the device for the AMF.

ii) Npcf_SMPolicyControl

It provides the SMF with policy related information to corresponding PDU session. It also have service operations such as

- Create: To create associtaion corresponding to particular PDU session used for PCF registration.

- Notify: If there is any policy cahnge to related PDU session, then the SMF will be notified by PCF.

- Update: To update that association or update notify by the PCF when there is no request.

- Delete: To delete the association corresponding to particular PDU session.

iii) Npcf_PolicyAuthentication

This is used to authorize an application function request and to create policies as requested by the authorized application function for the PDU session for which the application function session is bound.

iv) Npcf_BDTPolicy

To get the background data transfer policies based on the request via NEF from the application function. It updates the background data transfer policies on selection provided by application function.
