---
title: Acessar iosLobApp
description: Leia as propriedades e as relações do objeto iosLobApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 58a730dd09634a5f02547225fd23c3505dcdedea
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50157390"
---
# <a name="get-ioslobapp"></a><span data-ttu-id="dfe93-103">Acessar iosLobApp</span><span class="sxs-lookup"><span data-stu-id="dfe93-103">Get iosLobApp</span></span>

<span data-ttu-id="dfe93-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dfe93-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dfe93-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="dfe93-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dfe93-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="dfe93-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dfe93-107">Leia as propriedades e as relações do objeto [iosLobApp](../resources/intune-apps-ioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="dfe93-107">Read properties and relationships of the [iosLobApp](../resources/intune-apps-ioslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dfe93-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="dfe93-108">Prerequisites</span></span>
<span data-ttu-id="dfe93-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dfe93-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dfe93-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dfe93-111">Permission type</span></span>|<span data-ttu-id="dfe93-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="dfe93-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dfe93-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dfe93-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dfe93-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="dfe93-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="dfe93-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dfe93-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dfe93-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dfe93-116">Not supported.</span></span>|
|<span data-ttu-id="dfe93-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dfe93-117">Application</span></span>|<span data-ttu-id="dfe93-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="dfe93-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dfe93-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dfe93-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="dfe93-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="dfe93-120">Optional query parameters</span></span>
<span data-ttu-id="dfe93-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="dfe93-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dfe93-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dfe93-122">Request headers</span></span>
|<span data-ttu-id="dfe93-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dfe93-123">Header</span></span>|<span data-ttu-id="dfe93-124">Valor</span><span class="sxs-lookup"><span data-stu-id="dfe93-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dfe93-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="dfe93-125">Authorization</span></span>|<span data-ttu-id="dfe93-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dfe93-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dfe93-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="dfe93-127">Accept</span></span>|<span data-ttu-id="dfe93-128">application/json</span><span class="sxs-lookup"><span data-stu-id="dfe93-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dfe93-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dfe93-129">Request body</span></span>
<span data-ttu-id="dfe93-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dfe93-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dfe93-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="dfe93-131">Response</span></span>
<span data-ttu-id="dfe93-132">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [iosLobApp](../resources/intune-apps-ioslobapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dfe93-132">If successful, this method returns a `200 OK` response code and [iosLobApp](../resources/intune-apps-ioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dfe93-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dfe93-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="dfe93-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dfe93-134">Request</span></span>
<span data-ttu-id="dfe93-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dfe93-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="dfe93-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="dfe93-136">Response</span></span>
<span data-ttu-id="dfe93-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dfe93-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1779

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
    "dependentAppCount": 1,
    "supersedingAppCount": 3,
    "supersededAppCount": 2,
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
      "v12_0": true,
      "v13_0": true,
      "v14_0": true
    },
    "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
    "versionNumber": "Version Number value",
    "buildNumber": "Build Number value",
    "identityVersion": "Identity Version value"
  }
}
```




