---
title: Get microsoftStoreForBusinessApp
description: Ler propriedades e relações do objeto microsoftStoreForBusinessApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ae3fd3cecdc6b9fdbb5ce74be627e5ed8599d430
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30982753"
---
# <a name="get-microsoftstoreforbusinessapp"></a><span data-ttu-id="c1c46-103">Get microsoftStoreForBusinessApp</span><span class="sxs-lookup"><span data-stu-id="c1c46-103">Get microsoftStoreForBusinessApp</span></span>

> <span data-ttu-id="c1c46-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c1c46-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c1c46-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c1c46-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c1c46-106">Ler propriedades e relações do objeto [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span><span class="sxs-lookup"><span data-stu-id="c1c46-106">Read properties and relationships of the [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c1c46-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c1c46-107">Prerequisites</span></span>
<span data-ttu-id="c1c46-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c1c46-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1c46-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c1c46-110">Permission type</span></span>|<span data-ttu-id="c1c46-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c1c46-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c1c46-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c1c46-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c1c46-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c1c46-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="c1c46-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c1c46-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c1c46-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c1c46-115">Not supported.</span></span>|
|<span data-ttu-id="c1c46-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c1c46-116">Application</span></span>|<span data-ttu-id="c1c46-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c1c46-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c1c46-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c1c46-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c1c46-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c1c46-119">Optional query parameters</span></span>
<span data-ttu-id="c1c46-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c1c46-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c1c46-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c1c46-121">Request headers</span></span>
|<span data-ttu-id="c1c46-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c1c46-122">Header</span></span>|<span data-ttu-id="c1c46-123">Valor</span><span class="sxs-lookup"><span data-stu-id="c1c46-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c1c46-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="c1c46-124">Authorization</span></span>|<span data-ttu-id="c1c46-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c1c46-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c1c46-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c1c46-126">Accept</span></span>|<span data-ttu-id="c1c46-127">application/json</span><span class="sxs-lookup"><span data-stu-id="c1c46-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c1c46-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c1c46-128">Request body</span></span>
<span data-ttu-id="c1c46-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c1c46-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c1c46-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="c1c46-130">Response</span></span>
<span data-ttu-id="c1c46-131">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c1c46-131">If successful, this method returns a `200 OK` response code and [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1c46-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c1c46-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="c1c46-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c1c46-133">Request</span></span>
<span data-ttu-id="c1c46-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c1c46-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="c1c46-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="c1c46-135">Response</span></span>
<span data-ttu-id="c1c46-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c1c46-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1368

{
  "value": {
    "@odata.type": "#microsoft.graph.microsoftStoreForBusinessApp",
    "id": "f33358bc-58bc-f333-bc58-33f3bc5833f3",
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
    "productKey": "Product Key value",
    "licenseType": "online",
    "packageIdentityName": "Package Identity Name value",
    "licensingType": {
      "@odata.type": "microsoft.graph.vppLicensingType",
      "supportUserLicensing": true,
      "supportDeviceLicensing": true,
      "supportsUserLicensing": true,
      "supportsDeviceLicensing": true
    }
  }
}
```




