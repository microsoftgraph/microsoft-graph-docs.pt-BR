---
title: Acessar windowsMobileMSI
description: Leia as propriedades e as relações do objeto windowsMobileMSI.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a20b581879e6d99362149f3dd66135c8364f4eac
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37171957"
---
# <a name="get-windowsmobilemsi"></a><span data-ttu-id="d6178-103">Acessar windowsMobileMSI</span><span class="sxs-lookup"><span data-stu-id="d6178-103">Get windowsMobileMSI</span></span>

> <span data-ttu-id="d6178-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d6178-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d6178-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d6178-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d6178-106">Leia as propriedades e as relações do objeto [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md).</span><span class="sxs-lookup"><span data-stu-id="d6178-106">Read properties and relationships of the [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d6178-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d6178-107">Prerequisites</span></span>
<span data-ttu-id="d6178-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d6178-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6178-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d6178-110">Permission type</span></span>|<span data-ttu-id="d6178-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d6178-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d6178-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d6178-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d6178-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d6178-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="d6178-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d6178-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d6178-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d6178-115">Not supported.</span></span>|
|<span data-ttu-id="d6178-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d6178-116">Application</span></span>|<span data-ttu-id="d6178-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d6178-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d6178-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d6178-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d6178-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d6178-119">Optional query parameters</span></span>
<span data-ttu-id="d6178-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d6178-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d6178-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d6178-121">Request headers</span></span>
|<span data-ttu-id="d6178-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d6178-122">Header</span></span>|<span data-ttu-id="d6178-123">Valor</span><span class="sxs-lookup"><span data-stu-id="d6178-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d6178-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="d6178-124">Authorization</span></span>|<span data-ttu-id="d6178-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d6178-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d6178-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d6178-126">Accept</span></span>|<span data-ttu-id="d6178-127">application/json</span><span class="sxs-lookup"><span data-stu-id="d6178-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d6178-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d6178-128">Request body</span></span>
<span data-ttu-id="d6178-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d6178-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d6178-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="d6178-130">Response</span></span>
<span data-ttu-id="d6178-131">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d6178-131">If successful, this method returns a `200 OK` response code and [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d6178-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d6178-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="d6178-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d6178-133">Request</span></span>
<span data-ttu-id="d6178-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d6178-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="d6178-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="d6178-135">Response</span></span>
<span data-ttu-id="d6178-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d6178-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1325

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsMobileMSI",
    "id": "aa453e5d-3e5d-aa45-5d3e-45aa5d3e45aa",
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
    "committedContentVersion": "Committed Content Version value",
    "fileName": "File Name value",
    "size": 4,
    "commandLine": "Command Line value",
    "productCode": "Product Code value",
    "productVersion": "Product Version value",
    "ignoreVersionDetection": true,
    "identityVersion": "Identity Version value",
    "useDeviceContext": true
  }
}
```




