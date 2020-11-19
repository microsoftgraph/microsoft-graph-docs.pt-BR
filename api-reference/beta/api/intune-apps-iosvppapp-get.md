---
title: Acessar iosVppApp
description: Leia as propriedades e as relações do objeto iosVppApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6039c03d916b25e897b512a3ed02035d24b78c5a
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49252344"
---
# <a name="get-iosvppapp"></a><span data-ttu-id="f73db-103">Acessar iosVppApp</span><span class="sxs-lookup"><span data-stu-id="f73db-103">Get iosVppApp</span></span>

<span data-ttu-id="f73db-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f73db-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f73db-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f73db-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f73db-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f73db-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f73db-107">Leia as propriedades e as relações do objeto [iosVppApp](../resources/intune-apps-iosvppapp.md).</span><span class="sxs-lookup"><span data-stu-id="f73db-107">Read properties and relationships of the [iosVppApp](../resources/intune-apps-iosvppapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f73db-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f73db-108">Prerequisites</span></span>
<span data-ttu-id="f73db-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f73db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f73db-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f73db-111">Permission type</span></span>|<span data-ttu-id="f73db-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f73db-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f73db-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f73db-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f73db-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f73db-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="f73db-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f73db-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f73db-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f73db-116">Not supported.</span></span>|
|<span data-ttu-id="f73db-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f73db-117">Application</span></span>|<span data-ttu-id="f73db-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f73db-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f73db-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f73db-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f73db-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f73db-120">Optional query parameters</span></span>
<span data-ttu-id="f73db-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f73db-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f73db-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f73db-122">Request headers</span></span>
|<span data-ttu-id="f73db-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f73db-123">Header</span></span>|<span data-ttu-id="f73db-124">Valor</span><span class="sxs-lookup"><span data-stu-id="f73db-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f73db-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="f73db-125">Authorization</span></span>|<span data-ttu-id="f73db-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f73db-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f73db-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f73db-127">Accept</span></span>|<span data-ttu-id="f73db-128">application/json</span><span class="sxs-lookup"><span data-stu-id="f73db-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f73db-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f73db-129">Request body</span></span>
<span data-ttu-id="f73db-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f73db-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f73db-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="f73db-131">Response</span></span>
<span data-ttu-id="f73db-132">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [iosVppApp](../resources/intune-apps-iosvppapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f73db-132">If successful, this method returns a `200 OK` response code and [iosVppApp](../resources/intune-apps-iosvppapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f73db-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f73db-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="f73db-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f73db-134">Request</span></span>
<span data-ttu-id="f73db-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f73db-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="f73db-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="f73db-136">Response</span></span>
<span data-ttu-id="f73db-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f73db-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2371

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
    "dependentAppCount": 1,
    "supersedingAppCount": 3,
    "supersededAppCount": 2,
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




