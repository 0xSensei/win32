---
title: Service Principal Names
description: A service principal name (SPN) is a unique identifier of a service instance.
audience: developer
author: REDMOND\\markl
manager: REDMOND\\mbaldwin
ms.assetid: '54b02853-4097-4e37-b7a2-6b5cfd168ece'
ms.prod: 'windows-server-dev'
ms.technology: 'active-directory-domain-services'
ms.tgt_platform: multiple
keywords: ["Service Principal Names", "SPN see service principal names", "service principal name AD", "service principal name AD , about"]
---

# Service Principal Names

A service principal name (SPN) is a unique identifier of a service instance. SPNs are used by [Kerberos authentication](mutual-authentication-using-kerberos.md) to associate a service instance with a service logon account. This allows a client application to request that the service authenticate an account even if the client does not have the account name.

If you install multiple instances of a service on computers throughout a forest, each instance must have its own SPN. A given service instance can have multiple SPNs if there are multiple names that clients might use for authentication. For example, an SPN always includes the name of the host computer on which the service instance is running, so a service instance might register an SPN for each name or alias of its host. For more information about SPN format and composing a unique SPN, see [Name Formats for Unique SPNs](name-formats-for-unique-spns.md).

Before the Kerberos authentication service can use an SPN to authenticate a service, the SPN must be registered on the account object that the service instance uses to log on. A given SPN can be registered on only one account. For Win32 services, a service installer specifies the logon account when an instance of the service is installed. The installer then composes the SPNs and writes them as a property of the account object in Active Directory Domain Services. If the logon account of a service instance changes, the SPNs must be re-registered under the new account. For more information, see [How a Service Registers its SPNs](how-a-service-registers-its-spns.md).

When a client wants to connect to a service, it locates an instance of the service, composes an SPN for that instance, connects to the service, and presents the SPN for the service to authenticate. For more information, see [How Clients Compose a Service's SPN](how-clients-compose-a-serviceampaposs-spn.md).

## In this Section

## In this section

<dl> <dt>

[Name Formats for Unique SPNs](name-formats-for-unique-spns.md)
</dt> <dt>

[How a Service Composes its SPNs](how-a-service-composes-its-spns.md)
</dt> <dt>

[How a Service Registers its SPNs](how-a-service-registers-its-spns.md)
</dt> <dt>

[How Clients Compose a Service's SPN](how-clients-compose-a-serviceampaposs-spn.md)
</dt> </dl>

## Related topics

<dl> <dt>

[What is an SPN and why should you care?](http://blogs.msdn.com/b/autz_auth_stuff/archive/2011/04/28/what-is-spn-and-why-should-you-care.aspx)
</dt> <dt>

[Mutual Authentication Using Kerberos](mutual-authentication-using-kerberos.md)
</dt> </dl>

 

 



