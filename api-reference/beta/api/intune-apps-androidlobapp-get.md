---
title: Acessar androidLobApp
description: Leia as propriedades e as relações do objeto androidLobApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f5524e240cf3b6e2536e187410edc4512a1047a0
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/09/2019
ms.locfileid: "38081034"
---
# <a name="get-androidlobapp"></a><span data-ttu-id="982e3-103">Acessar androidLobApp</span><span class="sxs-lookup"><span data-stu-id="982e3-103">Get androidLobApp</span></span>

> <span data-ttu-id="982e3-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="982e3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="982e3-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="982e3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="982e3-106">Leia as propriedades e as relações do objeto [androidLobApp](../resources/intune-apps-androidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="982e3-106">Read properties and relationships of the [androidLobApp](../resources/intune-apps-androidlobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="982e3-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="982e3-107">Prerequisites</span></span>
<span data-ttu-id="982e3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="982e3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="982e3-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="982e3-110">Permission type</span></span>|<span data-ttu-id="982e3-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="982e3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="982e3-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="982e3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="982e3-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="982e3-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="982e3-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="982e3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="982e3-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="982e3-115">Not supported.</span></span>|
|<span data-ttu-id="982e3-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="982e3-116">Application</span></span>|<span data-ttu-id="982e3-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="982e3-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="982e3-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="982e3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="982e3-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="982e3-119">Optional query parameters</span></span>
<span data-ttu-id="982e3-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="982e3-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="982e3-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="982e3-121">Request headers</span></span>
|<span data-ttu-id="982e3-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="982e3-122">Header</span></span>|<span data-ttu-id="982e3-123">Valor</span><span class="sxs-lookup"><span data-stu-id="982e3-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="982e3-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="982e3-124">Authorization</span></span>|<span data-ttu-id="982e3-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="982e3-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="982e3-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="982e3-126">Accept</span></span>|<span data-ttu-id="982e3-127">application/json</span><span class="sxs-lookup"><span data-stu-id="982e3-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="982e3-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="982e3-128">Request body</span></span>
<span data-ttu-id="982e3-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="982e3-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="982e3-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="982e3-130">Response</span></span>
<span data-ttu-id="982e3-131">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [androidLobApp](../resources/intune-apps-androidlobapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="982e3-131">If successful, this method returns a `200 OK` response code and [androidLobApp](../resources/intune-apps-androidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="982e3-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="982e3-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="982e3-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="982e3-133">Request</span></span>
<span data-ttu-id="982e3-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="982e3-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="982e3-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="982e3-135">Response</span></span>
<span data-ttu-id="982e3-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="982e3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1704

{
  "value": {
    "@odata.type": "#microsoft.graph.androidLobApp",
    "id": "4b9a27d0-27d0-4b9a-d027-9a4bd0279a4b",
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
    "packageId": "Package Id value",
    "identityName": "Identity Name value",
    "minimumSupportedOperatingSystem": {
      "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
      "v4_0": true,
      "v4_0_3": true,
      "v4_1": true,
      "v4_2": true,
      "v4_3": true,
      "v4_4": true,
      "v5_0": true,
      "v5_1": true,
      "v6_0": true,
      "v7_0": true,
      "v7_1": true,
      "v8_0": true,
      "v8_1": true,
      "v9_0": true
    },
    "versionName": "Version Name value",
    "versionCode": "Version Code value",
    "identityVersion": "Identity Version value"
  }
}
```






