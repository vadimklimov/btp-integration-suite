<!-- loio9faf7cee8dc042569e6d539dc4879bf0 -->

# Request for Two-Way SSL Certificate

Request a two-way SSL certificate for the default domain of the virtual host of your API Management service.

> ### Note:  
> The default domain of the virtual host provided with your API Management service is secured with a one-way SSL certificate. For more information, see [Requesting a Custom Domain for a Virtual Host](requesting-a-custom-domain-for-a-virtual-host-6b9e5a3.md).

You can request for a two-way SSL certificate, which validates the identities of both the web server and the web client.



<a name="loio9faf7cee8dc042569e6d539dc4879bf0__section_mbk_544_1kb"/>

## Procedure

1.  Create an incident using the link [https://launchpad.support.sap.com/](https://launchpad.support.sap.com/)
2.  In the *Create Incident* window, expand the *Description* category and enter the following details:
    1.  The virtual host alias.

        > ### Note:  
        > For the default domain, this is the default virtual host alias.

    2.  Subdomain Name and ID: Go to *SAP BTP Cockpit* \> *<Your\_subaccount\>*. On the *Overview* page of your subaccount, make a note of the value marked against the *Subdomain* attribute as well as the *ID*.
    3.  Two-way SSL authentication : Enabled
    4.  An e-mail ID that you intend to use for sharing the secure drive link. The secure drive link is provided once you raise this incident, and you use the secure drive link to upload the public certificate, and the relevant chain certificate.
    5.  Component: **OPU-API-OD-OPS**

3.  Submit the incident.

