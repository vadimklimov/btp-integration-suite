<!-- loio8b7eb45224cb4162917ec7f5958d9c29 -->

<link rel="stylesheet" type="text/css" href="../css/sap-icons.css"/>

# Adding a Custom Message



## Context

You can add a custom message to a custom type system library.



## Procedure

1.  Navigate to the *Custom Type Systems* <span class="SAP-icons"></span> from the left pane of your application.

2.  Choose and open the custom type system and navigate to the *Messages* tab.

3.  This tab displays the list of uploaded custom messages. Choose *Add* to upload a custom message.

4.  Choose *Browse* and upload the XSD/WSDL file under the *XSD File*/*WSDL File* step.

    > ### Note:  
    > The maximum file size that you can upload is 10MB, with a maximum limit of 20000 nodes.

5.  The next step shows you all the messages present in your XSD/WSDL. Choose the required message from the *Messages* step.

6.  The details of the message will be auto-filled under the *Message Creation*step. You can verify and modify the details.

    > ### Note:  
    > -   The fields *Identifier*, *Namespace* and *Version* uniquely identify your message.
    > 
    > -   You can create multiple versions for a message with the same *Identifier* and *Namespace*.
    > -   If you upload a message with already existing *Identifier*, *Namespace* and *Version*, a new *Revision* of the message gets created. And, only the latest revision of the message gets displayed in the *Messages* list.

7.  Choose *Create*.




<a name="loio8b7eb45224cb4162917ec7f5958d9c29__result_azq_21h_spb"/>

## Results

The custom message is now successfully imported into the system.

<a name="concept_clb_1t5_czb"/>

<!-- concept\_clb\_1t5\_czb -->

## Extend Standard Message for Custom IDoc

The *Add* button has one more option *Extended Standard Message* for the custom IDocs type system. Using this option you can upload an IDoc message using an xsd file and then reference that message to a standard IDoc. Standard IDocs contain an enriched structural definition such as codelists, qualifiers, long-text documentation and DateTime information. The custom IDoc xsd files \(as downloaded from transaction WE60 of your S/4HANA backend system\) that you upload does not carry this additional information attached to these segment definitions. Now, with this option, these details \(codelists, qualifiers, long-text documentation and DateTime information\) are copied from the referenced standard IDoc to the custom IDoc.

> ### Note:  
> This additional information can only be copied for the standard segments \(from the standard IDoc\). Custom segments cannot be enriched using this option. For custom segments, you can manually enrich the MIG.

Follow the procedure below to know how.

1.  Choose *Add* and select *Extended Standard Message*.

2.  Choose *Browse* and upload the XSD file under the *XSD File* step.
3.  The next step shows you all the messages present in your XSD. Choose the required message from the *Messages* step.
4.  In the *Standard Type System* step, select the type system from which you want to choose the standard message.
5.  The *Standard Message* step displays the list of IDoc messages available in the selected type system. Select the required message from the list.
6.  The next step *Standard Versions* shows the list of versions available for the message that you chose. Select the version that you need to refer to your custom IDoc.
7.  The next step gives an overview of your selection. You can view a consolidated list of the standard message that you chose. Select *Create*.
8.  Select and open the newly created custom IDoc. You can now see the standard segments enriched with additional information.

