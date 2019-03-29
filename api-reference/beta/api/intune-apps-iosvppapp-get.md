---
title: Acessar iosVppApp
description: Leia as propriedades e as relações do objeto iosVppApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e21f92d721267b0e3111c8dc769fe917ebe04edb
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30978203"
---
# <a name="get-iosvppapp"></a><span data-ttu-id="25f69-103">Acessar iosVppApp</span><span class="sxs-lookup"><span data-stu-id="25f69-103">Get iosVppApp</span></span>

> <span data-ttu-id="25f69-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="25f69-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="25f69-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="25f69-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="25f69-106">Leia as propriedades e as relações do objeto [iosVppApp](../resources/intune-apps-iosvppapp.md).</span><span class="sxs-lookup"><span data-stu-id="25f69-106">Read properties and relationships of the [iosVppApp](../resources/intune-apps-iosvppapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="25f69-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="25f69-107">Prerequisites</span></span>
<span data-ttu-id="25f69-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="25f69-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="25f69-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="25f69-110">Permission type</span></span>|<span data-ttu-id="25f69-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="25f69-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="25f69-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="25f69-112">Delegated (work or school account)</span></span>|<span data-ttu-id="25f69-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="25f69-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="25f69-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="25f69-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="25f69-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="25f69-115">Not supported.</span></span>|
|<span data-ttu-id="25f69-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="25f69-116">Application</span></span>|<span data-ttu-id="25f69-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="25f69-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="25f69-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="25f69-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="25f69-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="25f69-119">Optional query parameters</span></span>
<span data-ttu-id="25f69-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="25f69-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="25f69-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="25f69-121">Request headers</span></span>
|<span data-ttu-id="25f69-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="25f69-122">Header</span></span>|<span data-ttu-id="25f69-123">Valor</span><span class="sxs-lookup"><span data-stu-id="25f69-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="25f69-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="25f69-124">Authorization</span></span>|<span data-ttu-id="25f69-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="25f69-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="25f69-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="25f69-126">Accept</span></span>|<span data-ttu-id="25f69-127">application/json</span><span class="sxs-lookup"><span data-stu-id="25f69-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="25f69-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="25f69-128">Request body</span></span>
<span data-ttu-id="25f69-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="25f69-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="25f69-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="25f69-130">Response</span></span>
<span data-ttu-id="25f69-131">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [iosVppApp](../resources/intune-apps-iosvppapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="25f69-131">If successful, this method returns a `200 OK` response code and [iosVppApp](../resources/intune-apps-iosvppapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="25f69-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="25f69-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="25f69-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="25f69-133">Request</span></span>
<span data-ttu-id="25f69-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="25f69-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="25f69-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="25f69-135">Response</span></span>
<span data-ttu-id="25f69-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="25f69-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2281

{
  "value": {
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
}
```




