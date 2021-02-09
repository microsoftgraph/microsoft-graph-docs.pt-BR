---
title: Acessar androidLobApp
description: Leia as propriedades e as relações do objeto androidLobApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f724be5b41e742d3d87a5ee45997ef3500b70138
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50157474"
---
# <a name="get-androidlobapp"></a><span data-ttu-id="dd274-103">Acessar androidLobApp</span><span class="sxs-lookup"><span data-stu-id="dd274-103">Get androidLobApp</span></span>

<span data-ttu-id="dd274-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dd274-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dd274-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="dd274-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dd274-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="dd274-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dd274-107">Leia as propriedades e as relações do objeto [androidLobApp](../resources/intune-apps-androidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="dd274-107">Read properties and relationships of the [androidLobApp](../resources/intune-apps-androidlobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dd274-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="dd274-108">Prerequisites</span></span>
<span data-ttu-id="dd274-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd274-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd274-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dd274-111">Permission type</span></span>|<span data-ttu-id="dd274-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="dd274-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dd274-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dd274-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dd274-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="dd274-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="dd274-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dd274-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dd274-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dd274-116">Not supported.</span></span>|
|<span data-ttu-id="dd274-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dd274-117">Application</span></span>|<span data-ttu-id="dd274-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="dd274-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dd274-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dd274-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="dd274-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="dd274-120">Optional query parameters</span></span>
<span data-ttu-id="dd274-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="dd274-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dd274-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dd274-122">Request headers</span></span>
|<span data-ttu-id="dd274-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dd274-123">Header</span></span>|<span data-ttu-id="dd274-124">Valor</span><span class="sxs-lookup"><span data-stu-id="dd274-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dd274-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="dd274-125">Authorization</span></span>|<span data-ttu-id="dd274-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dd274-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dd274-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="dd274-127">Accept</span></span>|<span data-ttu-id="dd274-128">application/json</span><span class="sxs-lookup"><span data-stu-id="dd274-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dd274-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dd274-129">Request body</span></span>
<span data-ttu-id="dd274-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dd274-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dd274-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="dd274-131">Response</span></span>
<span data-ttu-id="dd274-132">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [androidLobApp](../resources/intune-apps-androidlobapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dd274-132">If successful, this method returns a `200 OK` response code and [androidLobApp](../resources/intune-apps-androidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dd274-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dd274-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="dd274-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dd274-134">Request</span></span>
<span data-ttu-id="dd274-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dd274-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="dd274-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="dd274-136">Response</span></span>
<span data-ttu-id="dd274-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dd274-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1809

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
    "supersedingAppCount": 3,
    "supersededAppCount": 2,
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
      "v9_0": true,
      "v10_0": true,
      "v11_0": true
    },
    "versionName": "Version Name value",
    "versionCode": "Version Code value",
    "identityVersion": "Identity Version value"
  }
}
```




