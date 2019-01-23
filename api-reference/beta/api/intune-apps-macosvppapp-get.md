---
title: Obter macOsVppApp
description: Leia as propriedades e os relacionamentos do objeto macOsVppApp.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8ca675cf066ebe28619a3e5408c877f2b05a9414
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431243"
---
# <a name="get-macosvppapp"></a><span data-ttu-id="2f299-103">Obter macOsVppApp</span><span class="sxs-lookup"><span data-stu-id="2f299-103">Get macOsVppApp</span></span>

> <span data-ttu-id="2f299-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="2f299-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2f299-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="2f299-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2f299-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="2f299-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f299-107">Leia as propriedades e os relacionamentos do objeto [macOsVppApp](../resources/intune-apps-macosvppapp.md) .</span><span class="sxs-lookup"><span data-stu-id="2f299-107">Read properties and relationships of the [macOsVppApp](../resources/intune-apps-macosvppapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2f299-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2f299-108">Prerequisites</span></span>
<span data-ttu-id="2f299-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="2f299-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="2f299-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2f299-111">Permission type</span></span>|<span data-ttu-id="2f299-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2f299-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2f299-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2f299-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2f299-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="2f299-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="2f299-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2f299-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2f299-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2f299-116">Not supported.</span></span>|
|<span data-ttu-id="2f299-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2f299-117">Application</span></span>|<span data-ttu-id="2f299-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2f299-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2f299-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2f299-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2f299-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2f299-120">Optional query parameters</span></span>
<span data-ttu-id="2f299-121">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2f299-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2f299-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2f299-122">Request headers</span></span>
|<span data-ttu-id="2f299-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2f299-123">Header</span></span>|<span data-ttu-id="2f299-124">Valor</span><span class="sxs-lookup"><span data-stu-id="2f299-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2f299-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="2f299-125">Authorization</span></span>|<span data-ttu-id="2f299-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2f299-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2f299-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2f299-127">Accept</span></span>|<span data-ttu-id="2f299-128">application/json</span><span class="sxs-lookup"><span data-stu-id="2f299-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f299-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2f299-129">Request body</span></span>
<span data-ttu-id="2f299-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2f299-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2f299-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f299-131">Response</span></span>
<span data-ttu-id="2f299-132">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [macOsVppApp](../resources/intune-apps-macosvppapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2f299-132">If successful, this method returns a `200 OK` response code and [macOsVppApp](../resources/intune-apps-macosvppapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f299-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2f299-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="2f299-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2f299-134">Request</span></span>
<span data-ttu-id="2f299-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2f299-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="2f299-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f299-136">Response</span></span>
<span data-ttu-id="2f299-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2f299-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2141

{
  "value": {
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
}
```




