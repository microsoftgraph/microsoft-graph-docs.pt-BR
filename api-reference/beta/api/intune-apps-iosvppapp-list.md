---
title: Listar iosVppApps
description: Listar propriedades e relações dos objetos iosVppApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ba31286eb405c7d7e7699bef471a84e15e13de7c
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30966492"
---
# <a name="list-iosvppapps"></a><span data-ttu-id="70a9b-103">Listar iosVppApps</span><span class="sxs-lookup"><span data-stu-id="70a9b-103">List iosVppApps</span></span>

> <span data-ttu-id="70a9b-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="70a9b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="70a9b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="70a9b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="70a9b-106">Listar propriedades e relações dos objetos [iosVppApp](../resources/intune-apps-iosvppapp.md).</span><span class="sxs-lookup"><span data-stu-id="70a9b-106">List properties and relationships of the [iosVppApp](../resources/intune-apps-iosvppapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="70a9b-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="70a9b-107">Prerequisites</span></span>
<span data-ttu-id="70a9b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="70a9b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="70a9b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="70a9b-110">Permission type</span></span>|<span data-ttu-id="70a9b-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="70a9b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="70a9b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="70a9b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="70a9b-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="70a9b-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="70a9b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="70a9b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="70a9b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="70a9b-115">Not supported.</span></span>|
|<span data-ttu-id="70a9b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="70a9b-116">Application</span></span>|<span data-ttu-id="70a9b-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="70a9b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="70a9b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="70a9b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="70a9b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="70a9b-119">Request headers</span></span>
|<span data-ttu-id="70a9b-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="70a9b-120">Header</span></span>|<span data-ttu-id="70a9b-121">Valor</span><span class="sxs-lookup"><span data-stu-id="70a9b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="70a9b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="70a9b-122">Authorization</span></span>|<span data-ttu-id="70a9b-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="70a9b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="70a9b-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="70a9b-124">Accept</span></span>|<span data-ttu-id="70a9b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="70a9b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="70a9b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="70a9b-126">Request body</span></span>
<span data-ttu-id="70a9b-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="70a9b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="70a9b-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="70a9b-128">Response</span></span>
<span data-ttu-id="70a9b-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [iosVppApp](../resources/intune-apps-iosvppapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="70a9b-129">If successful, this method returns a `200 OK` response code and a collection of [iosVppApp](../resources/intune-apps-iosvppapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="70a9b-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="70a9b-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="70a9b-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="70a9b-131">Request</span></span>
<span data-ttu-id="70a9b-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="70a9b-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="70a9b-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="70a9b-133">Response</span></span>
<span data-ttu-id="70a9b-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="70a9b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2413

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
      "uploadState": 11,
      "publishingState": "processing",
      "isAssigned": true,
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "usedLicenseCount": 0,
      "totalLicenseCount": 1,
      "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "licensingType": {
        "@odata.type": "microsoft.graph.vppLicensingType",
        "supportUserLicensing": true,
        "supportDeviceLicensing": true,
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
      "bundleId": "Bundle Id value",
      "vppTokenId": "Vpp Token Id value",
      "revokeLicenseActionResults": [
        {
          "@odata.type": "microsoft.graph.iosVppAppRevokeLicensesActionResult",
          "userId": "User Id value",
          "managedDeviceId": "Managed Device Id value",
          "totalLicensesCount": 2,
          "failedLicensesCount": 3,
          "actionFailureReason": "appleFailure",
          "actionName": "Action Name value",
          "actionState": "pending",
          "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
          "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
        }
      ]
    }
  ]
}
```




