---
title: IMsRdpClient interface
description: Provides the methods and properties needed to configure and use the client control. Derives from the IMsTscAx interface.
ms.assetid: 6698c1d7-94d2-453c-96db-366113b95dd4
ms.tgt_platform: multiple
keywords:
- IMsRdpClient interface Remote Desktop Services
- IMsRdpClient interface Remote Desktop Services , described
topic_type:
- apiref
api_name:
- IMsRdpClient
api_location:
- MsTscAx.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
---

# IMsRdpClient interface

Provides the methods and properties needed to configure and use the client control. Derives from the [**IMsTscAx**](imstscax-interface.md) interface.

## Members

The **IMsRdpClient** interface inherits from [**IMsTscAx**](imstscax-interface.md). **IMsRdpClient** also has these types of members:

-   [Methods](#methods)
-   [Properties](#properties)

### Methods

The **IMsRdpClient** interface has these methods.



| Method                                                                    | Description                                                         |
|:--------------------------------------------------------------------------|:--------------------------------------------------------------------|
| [**GetVirtualChannelOptions**](imsrdpclient-getvirtualchanneloptions.md) | Retrieves the options set for a virtual channel.<br/>         |
| [**RequestClose**](imsrdpclient-requestclose.md)                         | Requests a graceful shutdown of the client control.<br/>      |
| [**SetVirtualChannelOptions**](imsrdpclient-setvirtualchanneloptions.md) | Sets the virtual channel options for the client control.<br/> |



 

### Properties

The **IMsRdpClient** interface has these properties.



| Property                                                                             | Access type           | Description                                                                                                                                                               |
|:-------------------------------------------------------------------------------------|:----------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [**AdvancedSettings2**](imsrdpclient-advancedsettings2.md)<br/>               | Read-only<br/>  | Pointer to the [**IMsRdpClientAdvancedSettings**](imsrdpclientadvancedsettings-interface.md) interface, used to set advanced settings for the client control.<br/> |
| [**ColorDepth**](imsrdpclient-colordepth.md)<br/>                             | Read/write<br/> | Color depth of the current control.<br/>                                                                                                                            |
| [**ExtendedDisconnectReason**](imsrdpclient-extendeddisconnectreason.md)<br/> | Read-only<br/>  | Extended information about the client control's reason for disconnection.<br/>                                                                                      |
| [**FullScreen**](imsrdpclient-fullscreen.md)<br/>                             | Read/write<br/> | Indicates whether the control is in full-screen mode.<br/>                                                                                                          |
| [**SecuredSettings2**](imsrdpclient-securedsettings2.md)<br/>                 | Read-only<br/>  | Pointer to the [**IMsRdpClientSecuredSettings**](imsrdpclientsecuredsettings-interface.md) interface, used to set secured settings for the client control.<br/>    |



 

## Remarks

The **IMsRdpClient** interface has been extended by the following interfaces, with each new interface inheriting all the methods and properties of the previous interfaces:

-   [**IMsRdpClient2**](imsrdpclient2.md)
-   [**IMsRdpClient3**](imsrdpclient3.md)
-   [**IMsRdpClient4**](imsrdpclient4.md)
-   [**IMsRdpClient5**](imsrdpclient5.md)
-   [**IMsRdpClient6**](imsrdpclient6.md)
-   [**IMsRdpClient7**](imsrdpclient7.md)
-   [**IMsRdpClient8**](imsrdpclient8.md)
-   [**IMsRdpClient9**](imsrdpclient9.md)
-   [**IMsRdpClient10**](imsrdpclient10.md)

For more information about Remote Desktop Web Connection, see [Requirements for Remote Desktop Web Connection](requirements-for-remote-desktop-web-connection.md).

## Requirements



| Requirement | Value |
|-------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows Vista<br/>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| Minimum supported server<br/> | Windows Server 2008<br/>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| Type library<br/>             | <dl> <dt>MsTscAx.dll</dt> </dl>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| DLL<br/>                      | <dl> <dt>MsTscAx.dll</dt> </dl>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| CLSID<br/>                    | CLSID\_MsRdpClient is defined as 791fa017-2de3-492e-acc5-53c67a2b94d0<br/> CLSID\_MsRdpClient10 is defined as C0EFA91A-EEB7-41C7-97FA-F0ED645EFB24<br/> CLSID\_MsRdpClient10NotSafeForScripting is defined as A0C63C30-F08D-4AB4-907C-34905D770C7D<br/> CLSID\_MsRdpClient2 is defined as 9059F30F-4EB1-4BD2-9FDC-36F43A218F4A<br/> CLSID\_MsRdpClient2a is defined as 971127BB-259F-48C2-BD75-5F97A3331551<br/> CLSID\_MsRdpClient2NotSafeForScripting is defined as 3523C2FB-4031-44E4-9A3B-F1E94986EE7F<br/> CLSID\_MsRdpClient3 is defined as 7584C670-2274-4EFB-B00B-D6AABA6D3850<br/> CLSID\_MsRdpClient3a is defined as 6A6F4B83-45C5-4CA9-BDD9-0D81C12295E4<br/> CLSID\_MsRdpClient3NotSafeForScripting is defined as ACE575FD-1FCF-4074-9401-EBAB990FA9DE<br/> CLSID\_MsRdpClient4 is defined as 4EDCB26C-D24C-4E72-AF07-B576699AC0DE<br/> CLSID\_MsRdpClient4a is defined as 54CE37E0-9834-41AE-9896-4DAB69DC022B<br/> CLSID\_MsRdpClient4NotSafeForScripting is defined as 6AE29350-321B-42BE-BBE5-12FB5270C0DE<br/> CLSID\_MsRdpClient5 is defined as 4EB89FF4-7F78-4A0F-8B8D-2BF02E94E4B2<br/> CLSID\_MsRdpClient5NotSafeForScripting is defined as 4EB2F086-C818-447E-B32C-C51CE2B30D31<br/> CLSID\_MsRdpClient6 is defined as 7390F3D8-0439-4C05-91E3-CF5CB290C3D0<br/> CLSID\_MsRdpClient6NotSafeForScripting is defined as D2EA46A7-C2BF-426B-AF24-E19C44456399<br/> CLSID\_MsRdpClient7 is defined as A9D7038D-B5ED-472E-9C47-94BEA90A5910<br/> CLSID\_MsRdpClient7NotSafeForScripting is defined as 54D38BF7-B1EF-4479-9674-1BD6EA465258<br/> CLSID\_MsRdpClient8 is defined as 5F681803-2900-4C43-A1CC-CF405404A676<br/> CLSID\_MsRdpClient8NotSafeForScripting is defined as A3BC03A0-041D-42E3-AD22-882B7865C9C5<br/> CLSID\_MsRdpClient9 is defined as 301B94BA-5D25-4A12-BFFE-3B6E7A616585<br/> CLSID\_MsRdpClient9NotSafeForScripting is defined as 8B918B82-7985-4C24-89DF-C33AD2BBFBCD<br/> CLSID\_MsRdpClientNotSafeForScripting is defined as 7CACBD7B-0D99-468F-AC33-22E495C0AFE5<br/> CLSID\_MsTscAx is defined as 1FB464C8-09BB-4017-A2F5-EB742F04392F<br/> CLSID\_MsTscAxNotSafeForScripting is defined as A41A4187-5A86-4E26-B40A-856F9035D9CB<br/> |
| IID<br/>                      | IID\_IMsRdpClient is defined as 92b4a539-7115-4b7c-a5a9-e5d9efc2780a<br/>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |



## See also

<dl> <dt>

[**IMsTscAx**](imstscax-interface.md)
</dt> <dt>

[Remote Desktop Web Connection Reference](remote-desktop-web-connection-reference.md)
</dt> </dl>

 

 





