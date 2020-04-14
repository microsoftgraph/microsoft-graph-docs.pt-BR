---
title: Get microsoftStoreForBusinessApp
description: Ler propriedades e relações do objeto microsoftStoreForBusinessApp.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 24d5b4fb4f54f44db92f8831b7e7bf69e3f79cc4
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43405133"
---
# <a name="get-microsoftstoreforbusinessapp"></a><span data-ttu-id="63294-103">Get microsoftStoreForBusinessApp</span><span class="sxs-lookup"><span data-stu-id="63294-103">Get microsoftStoreForBusinessApp</span></span>

<span data-ttu-id="63294-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="63294-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="63294-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="63294-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="63294-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="63294-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="63294-107">Ler propriedades e relações do objeto [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span><span class="sxs-lookup"><span data-stu-id="63294-107">Read properties and relationships of the [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="63294-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="63294-108">Prerequisites</span></span>
<span data-ttu-id="63294-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="63294-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="63294-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="63294-111">Permission type</span></span>|<span data-ttu-id="63294-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="63294-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="63294-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="63294-113">Delegated (work or school account)</span></span>|<span data-ttu-id="63294-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="63294-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="63294-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="63294-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="63294-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="63294-116">Not supported.</span></span>|
|<span data-ttu-id="63294-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="63294-117">Application</span></span>|<span data-ttu-id="63294-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="63294-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="63294-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="63294-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="63294-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="63294-120">Optional query parameters</span></span>
<span data-ttu-id="63294-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="63294-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="63294-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="63294-122">Request headers</span></span>
|<span data-ttu-id="63294-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="63294-123">Header</span></span>|<span data-ttu-id="63294-124">Valor</span><span class="sxs-lookup"><span data-stu-id="63294-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="63294-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="63294-125">Authorization</span></span>|<span data-ttu-id="63294-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="63294-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="63294-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="63294-127">Accept</span></span>|<span data-ttu-id="63294-128">application/json</span><span class="sxs-lookup"><span data-stu-id="63294-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="63294-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="63294-129">Request body</span></span>
<span data-ttu-id="63294-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="63294-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="63294-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="63294-131">Response</span></span>
<span data-ttu-id="63294-132">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="63294-132">If successful, this method returns a `200 OK` response code and [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="63294-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="63294-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="63294-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="63294-134">Request</span></span>
<span data-ttu-id="63294-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="63294-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="63294-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="63294-136">Response</span></span>
<span data-ttu-id="63294-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="63294-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1397

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
    "dependentAppCount": 1,
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



