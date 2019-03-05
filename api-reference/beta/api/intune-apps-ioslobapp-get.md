---
title: Acessar iosLobApp
description: Leia as propriedades e as relações do objeto iosLobApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2c50a9a839c218a66492c245e34a4833b72ba248
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30160883"
---
# <a name="get-ioslobapp"></a><span data-ttu-id="61591-103">Acessar iosLobApp</span><span class="sxs-lookup"><span data-stu-id="61591-103">Get iosLobApp</span></span>

> <span data-ttu-id="61591-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="61591-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="61591-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="61591-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="61591-106">Leia as propriedades e as relações do objeto [iosLobApp](../resources/intune-apps-ioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="61591-106">Read properties and relationships of the [iosLobApp](../resources/intune-apps-ioslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="61591-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="61591-107">Prerequisites</span></span>
<span data-ttu-id="61591-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="61591-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="61591-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="61591-110">Permission type</span></span>|<span data-ttu-id="61591-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="61591-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="61591-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="61591-112">Delegated (work or school account)</span></span>|<span data-ttu-id="61591-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="61591-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="61591-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="61591-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="61591-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="61591-115">Not supported.</span></span>|
|<span data-ttu-id="61591-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="61591-116">Application</span></span>|<span data-ttu-id="61591-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="61591-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="61591-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="61591-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="61591-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="61591-119">Optional query parameters</span></span>
<span data-ttu-id="61591-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="61591-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="61591-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="61591-121">Request headers</span></span>
|<span data-ttu-id="61591-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="61591-122">Header</span></span>|<span data-ttu-id="61591-123">Valor</span><span class="sxs-lookup"><span data-stu-id="61591-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="61591-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="61591-124">Authorization</span></span>|<span data-ttu-id="61591-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="61591-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="61591-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="61591-126">Accept</span></span>|<span data-ttu-id="61591-127">application/json</span><span class="sxs-lookup"><span data-stu-id="61591-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="61591-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="61591-128">Request body</span></span>
<span data-ttu-id="61591-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="61591-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="61591-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="61591-130">Response</span></span>
<span data-ttu-id="61591-131">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [iosLobApp](../resources/intune-apps-ioslobapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="61591-131">If successful, this method returns a `200 OK` response code and [iosLobApp](../resources/intune-apps-ioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="61591-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="61591-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="61591-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="61591-133">Request</span></span>
<span data-ttu-id="61591-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="61591-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="61591-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="61591-135">Response</span></span>
<span data-ttu-id="61591-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="61591-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1645

{
  "value": {
    "@odata.type": "#microsoft.graph.iosLobApp",
    "id": "b34052ea-52ea-b340-ea52-40b3ea5240b3",
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
    "committedContentVersion": "Committed Content Version value",
    "fileName": "File Name value",
    "size": 4,
    "bundleId": "Bundle Id value",
    "applicableDeviceType": {
      "@odata.type": "microsoft.graph.iosDeviceType",
      "iPad": true,
      "iPhoneAndIPod": true
    },
    "minimumSupportedOperatingSystem": {
      "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
      "v8_0": true,
      "v9_0": true,
      "v10_0": true,
      "v11_0": true,
      "v12_0": true
    },
    "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
    "versionNumber": "Version Number value",
    "buildNumber": "Build Number value",
    "identityVersion": "Identity Version value"
  }
}
```




