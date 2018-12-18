---
title: Listar managedIOSLobApps
description: Listar propriedades e relações dos objetos managedIOSLobApp.
author: tfitzmac
ms.openlocfilehash: 3dc053035c66fd7be477d6d8991247d5137b23f9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27331448"
---
# <a name="list-managedioslobapps"></a><span data-ttu-id="16e28-103">Listar managedIOSLobApps</span><span class="sxs-lookup"><span data-stu-id="16e28-103">List managedIOSLobApps</span></span>

> <span data-ttu-id="16e28-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="16e28-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="16e28-105">Listar propriedades e relações dos objetos [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="16e28-105">List properties and relationships of the [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="16e28-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="16e28-106">Prerequisites</span></span>
<span data-ttu-id="16e28-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="16e28-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16e28-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="16e28-109">Permission type</span></span>|<span data-ttu-id="16e28-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="16e28-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="16e28-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="16e28-111">Delegated (work or school account)</span></span>|<span data-ttu-id="16e28-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="16e28-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="16e28-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="16e28-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="16e28-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="16e28-114">Not supported.</span></span>|
|<span data-ttu-id="16e28-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="16e28-115">Application</span></span>|<span data-ttu-id="16e28-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="16e28-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="16e28-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="16e28-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="16e28-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="16e28-118">Request headers</span></span>
|<span data-ttu-id="16e28-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="16e28-119">Header</span></span>|<span data-ttu-id="16e28-120">Valor</span><span class="sxs-lookup"><span data-stu-id="16e28-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="16e28-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="16e28-121">Authorization</span></span>|<span data-ttu-id="16e28-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="16e28-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="16e28-123">Accept</span><span class="sxs-lookup"><span data-stu-id="16e28-123">Accept</span></span>|<span data-ttu-id="16e28-124">application/json</span><span class="sxs-lookup"><span data-stu-id="16e28-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="16e28-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="16e28-125">Request body</span></span>
<span data-ttu-id="16e28-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="16e28-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="16e28-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="16e28-127">Response</span></span>
<span data-ttu-id="16e28-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="16e28-128">If successful, this method returns a `200 OK` response code and a collection of [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16e28-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="16e28-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="16e28-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="16e28-130">Request</span></span>
<span data-ttu-id="16e28-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="16e28-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="16e28-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="16e28-132">Response</span></span>
<span data-ttu-id="16e28-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="16e28-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1656

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedIOSLobApp",
      "id": "8f59792d-792d-8f59-2d79-598f2d79598f",
      "displayName": "Display Name value",
      "description": "Description value",
      "publisher": "Publisher value",
      "largeIcon": {
        "@odata.type": "microsoft.graph.mimeContent",
        "type": "Type value",
        "value": "dmFsdWU="
      },
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "isFeatured": true,
      "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
      "informationUrl": "https://example.com/informationUrl/",
      "owner": "Owner value",
      "developer": "Developer value",
      "notes": "Notes value",
      "publishingState": "processing",
      "appAvailability": "lineOfBusiness",
      "version": "Version value",
      "committedContentVersion": "Committed Content Version value",
      "fileName": "File Name value",
      "size": 4,
      "bundleId": "Bundle Id value",
      "applicableDeviceType": {
        "@odata.type": "microsoft.graph.iosDeviceType",
        "iPad": true,
        "iPhoneAndIPod": true
      },
      "minimumSupportedOperatingSystem": {
        "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
        "v8_0": true,
        "v9_0": true,
        "v10_0": true,
        "v11_0": true,
        "v12_0": true
      },
      "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
      "versionNumber": "Version Number value",
      "buildNumber": "Build Number value"
    }
  ]
}
```



