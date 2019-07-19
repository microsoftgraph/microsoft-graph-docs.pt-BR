---
title: Get windowsUniversalAppX
description: Ler propriedades e relações do objeto windowsUniversalAppX.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a720a0c4ff0f9f4ae0d068a951543fb52439bc55
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34972736"
---
# <a name="get-windowsuniversalappx"></a><span data-ttu-id="73354-103">Get windowsUniversalAppX</span><span class="sxs-lookup"><span data-stu-id="73354-103">Get windowsUniversalAppX</span></span>

> <span data-ttu-id="73354-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="73354-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="73354-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="73354-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="73354-106">Ler propriedades e relações do objeto [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md).</span><span class="sxs-lookup"><span data-stu-id="73354-106">Read properties and relationships of the [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="73354-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="73354-107">Prerequisites</span></span>
<span data-ttu-id="73354-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="73354-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73354-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="73354-110">Permission type</span></span>|<span data-ttu-id="73354-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="73354-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="73354-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="73354-112">Delegated (work or school account)</span></span>|<span data-ttu-id="73354-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="73354-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="73354-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="73354-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="73354-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="73354-115">Not supported.</span></span>|
|<span data-ttu-id="73354-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="73354-116">Application</span></span>|<span data-ttu-id="73354-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="73354-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="73354-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="73354-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="73354-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="73354-119">Optional query parameters</span></span>
<span data-ttu-id="73354-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="73354-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="73354-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="73354-121">Request headers</span></span>
|<span data-ttu-id="73354-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="73354-122">Header</span></span>|<span data-ttu-id="73354-123">Valor</span><span class="sxs-lookup"><span data-stu-id="73354-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="73354-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="73354-124">Authorization</span></span>|<span data-ttu-id="73354-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="73354-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="73354-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="73354-126">Accept</span></span>|<span data-ttu-id="73354-127">application/json</span><span class="sxs-lookup"><span data-stu-id="73354-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="73354-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="73354-128">Request body</span></span>
<span data-ttu-id="73354-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="73354-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="73354-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="73354-130">Response</span></span>
<span data-ttu-id="73354-131">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="73354-131">If successful, this method returns a `200 OK` response code and [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73354-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="73354-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="73354-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="73354-133">Request</span></span>
<span data-ttu-id="73354-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="73354-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="73354-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="73354-135">Response</span></span>
<span data-ttu-id="73354-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="73354-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1746

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsUniversalAppX",
    "id": "4bc47eba-7eba-4bc4-ba7e-c44bba7ec44b",
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
    "applicableArchitectures": "x86",
    "applicableDeviceTypes": "desktop",
    "identityName": "Identity Name value",
    "identityPublisherHash": "Identity Publisher Hash value",
    "identityResourceIdentifier": "Identity Resource Identifier value",
    "isBundle": true,
    "minimumSupportedOperatingSystem": {
      "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
      "v8_0": true,
      "v8_1": true,
      "v10_0": true,
      "v10_1607": true,
      "v10_1703": true,
      "v10_1709": true,
      "v10_1803": true,
      "v10_1809": true,
      "v10_1903": true
    },
    "identityVersion": "Identity Version value"
  }
}
```





