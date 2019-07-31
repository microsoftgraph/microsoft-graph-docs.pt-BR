---
title: Acessar managedAndroidLobApp
description: Leia as propriedades e as relações do objeto managedAndroidLobApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0a12aa8a458a7246b0dffa2d5b0ba68b9d7f56ae
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35961865"
---
# <a name="get-managedandroidlobapp"></a><span data-ttu-id="e5081-103">Acessar managedAndroidLobApp</span><span class="sxs-lookup"><span data-stu-id="e5081-103">Get managedAndroidLobApp</span></span>

> <span data-ttu-id="e5081-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e5081-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e5081-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e5081-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e5081-106">Leia as propriedades e as relações do objeto [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="e5081-106">Read properties and relationships of the [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e5081-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e5081-107">Prerequisites</span></span>
<span data-ttu-id="e5081-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e5081-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5081-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e5081-110">Permission type</span></span>|<span data-ttu-id="e5081-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e5081-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e5081-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e5081-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e5081-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e5081-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="e5081-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e5081-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e5081-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e5081-115">Not supported.</span></span>|
|<span data-ttu-id="e5081-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e5081-116">Application</span></span>|<span data-ttu-id="e5081-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e5081-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e5081-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e5081-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e5081-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e5081-119">Optional query parameters</span></span>
<span data-ttu-id="e5081-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e5081-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e5081-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e5081-121">Request headers</span></span>
|<span data-ttu-id="e5081-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e5081-122">Header</span></span>|<span data-ttu-id="e5081-123">Valor</span><span class="sxs-lookup"><span data-stu-id="e5081-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e5081-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="e5081-124">Authorization</span></span>|<span data-ttu-id="e5081-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e5081-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e5081-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e5081-126">Accept</span></span>|<span data-ttu-id="e5081-127">application/json</span><span class="sxs-lookup"><span data-stu-id="e5081-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e5081-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e5081-128">Request body</span></span>
<span data-ttu-id="e5081-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e5081-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e5081-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="e5081-130">Response</span></span>
<span data-ttu-id="e5081-131">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e5081-131">If successful, this method returns a `200 OK` response code and [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e5081-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e5081-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="e5081-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e5081-133">Request</span></span>
<span data-ttu-id="e5081-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e5081-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="e5081-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="e5081-135">Response</span></span>
<span data-ttu-id="e5081-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e5081-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1786

{
  "value": {
    "@odata.type": "#microsoft.graph.managedAndroidLobApp",
    "id": "802b7ed3-7ed3-802b-d37e-2b80d37e2b80",
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
    "appAvailability": "lineOfBusiness",
    "version": "Version value",
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





