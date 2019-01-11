---
title: Listar iosVppApps
description: Listar propriedades e relações dos objetos iosVppApp.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 7742a542f97a9135cb15c7744badcd1284c62c98
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27843145"
---
# <a name="list-iosvppapps"></a><span data-ttu-id="3d856-103">Listar iosVppApps</span><span class="sxs-lookup"><span data-stu-id="3d856-103">List iosVppApps</span></span>

> <span data-ttu-id="3d856-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="3d856-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3d856-105">Listar propriedades e relações dos objetos [iosVppApp](../resources/intune-apps-iosvppapp.md).</span><span class="sxs-lookup"><span data-stu-id="3d856-105">List properties and relationships of the [iosVppApp](../resources/intune-apps-iosvppapp.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3d856-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3d856-106">Prerequisites</span></span>
<span data-ttu-id="3d856-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3d856-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3d856-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3d856-109">Permission type</span></span>|<span data-ttu-id="3d856-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3d856-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3d856-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3d856-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3d856-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="3d856-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="3d856-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3d856-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3d856-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3d856-114">Not supported.</span></span>|
|<span data-ttu-id="3d856-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3d856-115">Application</span></span>|<span data-ttu-id="3d856-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3d856-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3d856-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3d856-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="3d856-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3d856-118">Request headers</span></span>
|<span data-ttu-id="3d856-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3d856-119">Header</span></span>|<span data-ttu-id="3d856-120">Valor</span><span class="sxs-lookup"><span data-stu-id="3d856-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3d856-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="3d856-121">Authorization</span></span>|<span data-ttu-id="3d856-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3d856-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3d856-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3d856-123">Accept</span></span>|<span data-ttu-id="3d856-124">application/json</span><span class="sxs-lookup"><span data-stu-id="3d856-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3d856-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3d856-125">Request body</span></span>
<span data-ttu-id="3d856-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3d856-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3d856-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="3d856-127">Response</span></span>
<span data-ttu-id="3d856-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [iosVppApp](../resources/intune-apps-iosvppapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3d856-128">If successful, this method returns a `200 OK` response code and a collection of [iosVppApp](../resources/intune-apps-iosvppapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3d856-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3d856-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="3d856-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3d856-130">Request</span></span>
<span data-ttu-id="3d856-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3d856-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="3d856-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="3d856-132">Response</span></span>
<span data-ttu-id="3d856-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3d856-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1575

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosVppApp",
      "id": "a0ac9b6f-9b6f-a0ac-6f9b-aca06f9baca0",
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
      "usedLicenseCount": 0,
      "totalLicenseCount": 1,
      "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "licensingType": {
        "@odata.type": "microsoft.graph.vppLicensingType",
        "supportsUserLicensing": true,
        "supportsDeviceLicensing": true
      },
      "applicableDeviceType": {
        "@odata.type": "microsoft.graph.iosDeviceType",
        "iPad": true,
        "iPhoneAndIPod": true
      },
      "vppTokenOrganizationName": "Vpp Token Organization Name value",
      "vppTokenAccountType": "education",
      "vppTokenAppleId": "Vpp Token Apple Id value",
      "bundleId": "Bundle Id value"
    }
  ]
}
```



