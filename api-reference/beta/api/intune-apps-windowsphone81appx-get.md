---
title: Obter windowsPhone81AppX
description: Leia as propriedades e as relações do objeto windowsPhone81AppX.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f34aeb21dbfb5d19e7757057f2ef79dcd2aec344
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34973079"
---
# <a name="get-windowsphone81appx"></a><span data-ttu-id="7d4f8-103">Obter windowsPhone81AppX</span><span class="sxs-lookup"><span data-stu-id="7d4f8-103">Get windowsPhone81AppX</span></span>

> <span data-ttu-id="7d4f8-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7d4f8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7d4f8-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7d4f8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7d4f8-106">Leia as propriedades e as relações do objeto [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) .</span><span class="sxs-lookup"><span data-stu-id="7d4f8-106">Read properties and relationships of the [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7d4f8-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7d4f8-107">Prerequisites</span></span>
<span data-ttu-id="7d4f8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7d4f8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7d4f8-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7d4f8-110">Permission type</span></span>|<span data-ttu-id="7d4f8-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7d4f8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7d4f8-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7d4f8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7d4f8-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="7d4f8-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="7d4f8-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7d4f8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7d4f8-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7d4f8-115">Not supported.</span></span>|
|<span data-ttu-id="7d4f8-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7d4f8-116">Application</span></span>|<span data-ttu-id="7d4f8-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7d4f8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7d4f8-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7d4f8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7d4f8-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7d4f8-119">Optional query parameters</span></span>
<span data-ttu-id="7d4f8-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7d4f8-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7d4f8-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7d4f8-121">Request headers</span></span>
|<span data-ttu-id="7d4f8-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7d4f8-122">Header</span></span>|<span data-ttu-id="7d4f8-123">Valor</span><span class="sxs-lookup"><span data-stu-id="7d4f8-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7d4f8-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="7d4f8-124">Authorization</span></span>|<span data-ttu-id="7d4f8-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7d4f8-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7d4f8-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7d4f8-126">Accept</span></span>|<span data-ttu-id="7d4f8-127">application/json</span><span class="sxs-lookup"><span data-stu-id="7d4f8-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7d4f8-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7d4f8-128">Request body</span></span>
<span data-ttu-id="7d4f8-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7d4f8-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7d4f8-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d4f8-130">Response</span></span>
<span data-ttu-id="7d4f8-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7d4f8-131">If successful, this method returns a `200 OK` response code and [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7d4f8-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7d4f8-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="7d4f8-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7d4f8-133">Request</span></span>
<span data-ttu-id="7d4f8-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7d4f8-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="7d4f8-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d4f8-135">Response</span></span>
<span data-ttu-id="7d4f8-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7d4f8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1798

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsPhone81AppX",
    "id": "4ff27f80-7f80-4ff2-807f-f24f807ff24f",
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
    "identityName": "Identity Name value",
    "identityPublisherHash": "Identity Publisher Hash value",
    "identityResourceIdentifier": "Identity Resource Identifier value",
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
    "phoneProductIdentifier": "Phone Product Identifier value",
    "phonePublisherId": "Phone Publisher Id value",
    "identityVersion": "Identity Version value"
  }
}
```





