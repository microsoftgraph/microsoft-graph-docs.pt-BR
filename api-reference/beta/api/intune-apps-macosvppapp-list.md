---
title: Listar macOsVppApps
description: Listar Propriedades e relações dos objetos macOsVppApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9cc9f6b92a927aefa8ce30b248bd3a2f1cc39aaf
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34975172"
---
# <a name="list-macosvppapps"></a><span data-ttu-id="81348-103">Listar macOsVppApps</span><span class="sxs-lookup"><span data-stu-id="81348-103">List macOsVppApps</span></span>

> <span data-ttu-id="81348-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="81348-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="81348-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="81348-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="81348-106">Listar Propriedades e relações dos objetos [macOsVppApp](../resources/intune-apps-macosvppapp.md) .</span><span class="sxs-lookup"><span data-stu-id="81348-106">List properties and relationships of the [macOsVppApp](../resources/intune-apps-macosvppapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="81348-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="81348-107">Prerequisites</span></span>
<span data-ttu-id="81348-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="81348-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="81348-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="81348-110">Permission type</span></span>|<span data-ttu-id="81348-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="81348-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="81348-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="81348-112">Delegated (work or school account)</span></span>|<span data-ttu-id="81348-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="81348-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="81348-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="81348-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="81348-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="81348-115">Not supported.</span></span>|
|<span data-ttu-id="81348-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="81348-116">Application</span></span>|<span data-ttu-id="81348-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="81348-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="81348-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="81348-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="81348-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="81348-119">Request headers</span></span>
|<span data-ttu-id="81348-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="81348-120">Header</span></span>|<span data-ttu-id="81348-121">Valor</span><span class="sxs-lookup"><span data-stu-id="81348-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="81348-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="81348-122">Authorization</span></span>|<span data-ttu-id="81348-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="81348-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="81348-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="81348-124">Accept</span></span>|<span data-ttu-id="81348-125">application/json</span><span class="sxs-lookup"><span data-stu-id="81348-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="81348-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="81348-126">Request body</span></span>
<span data-ttu-id="81348-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="81348-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="81348-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="81348-128">Response</span></span>
<span data-ttu-id="81348-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [macOsVppApp](../resources/intune-apps-macosvppapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="81348-129">If successful, this method returns a `200 OK` response code and a collection of [macOsVppApp](../resources/intune-apps-macosvppapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="81348-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="81348-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="81348-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="81348-131">Request</span></span>
<span data-ttu-id="81348-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="81348-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="81348-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="81348-133">Response</span></span>
<span data-ttu-id="81348-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="81348-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2294

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.macOsVppApp",
      "id": "10b95265-5265-10b9-6552-b9106552b910",
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
      "dependentAppCount": 1,
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
      "vppTokenOrganizationName": "Vpp Token Organization Name value",
      "vppTokenAccountType": "education",
      "vppTokenAppleId": "Vpp Token Apple Id value",
      "bundleId": "Bundle Id value",
      "vppTokenId": "Vpp Token Id value",
      "revokeLicenseActionResults": [
        {
          "@odata.type": "microsoft.graph.macOsVppAppRevokeLicensesActionResult",
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





