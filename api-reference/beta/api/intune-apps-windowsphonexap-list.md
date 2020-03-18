---
title: Listar windowsPhoneXAPs
description: Listar Propriedades e relações dos objetos windowsPhoneXAP.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0f70a340c4409452aade86f803bfd6d1dd984095
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42760722"
---
# <a name="list-windowsphonexaps"></a><span data-ttu-id="32f66-103">Listar windowsPhoneXAPs</span><span class="sxs-lookup"><span data-stu-id="32f66-103">List windowsPhoneXAPs</span></span>

> <span data-ttu-id="32f66-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="32f66-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="32f66-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="32f66-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="32f66-106">Listar Propriedades e relações dos objetos [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) .</span><span class="sxs-lookup"><span data-stu-id="32f66-106">List properties and relationships of the [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="32f66-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="32f66-107">Prerequisites</span></span>
<span data-ttu-id="32f66-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="32f66-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="32f66-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="32f66-110">Permission type</span></span>|<span data-ttu-id="32f66-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="32f66-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="32f66-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="32f66-112">Delegated (work or school account)</span></span>|<span data-ttu-id="32f66-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="32f66-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="32f66-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="32f66-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="32f66-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="32f66-115">Not supported.</span></span>|
|<span data-ttu-id="32f66-116">Application</span><span class="sxs-lookup"><span data-stu-id="32f66-116">Application</span></span>|<span data-ttu-id="32f66-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="32f66-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="32f66-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="32f66-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="32f66-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="32f66-119">Request headers</span></span>
|<span data-ttu-id="32f66-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="32f66-120">Header</span></span>|<span data-ttu-id="32f66-121">Valor</span><span class="sxs-lookup"><span data-stu-id="32f66-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="32f66-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="32f66-122">Authorization</span></span>|<span data-ttu-id="32f66-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="32f66-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="32f66-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="32f66-124">Accept</span></span>|<span data-ttu-id="32f66-125">application/json</span><span class="sxs-lookup"><span data-stu-id="32f66-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="32f66-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="32f66-126">Request body</span></span>
<span data-ttu-id="32f66-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="32f66-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="32f66-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="32f66-128">Response</span></span>
<span data-ttu-id="32f66-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="32f66-129">If successful, this method returns a `200 OK` response code and a collection of [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="32f66-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="32f66-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="32f66-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="32f66-131">Request</span></span>
<span data-ttu-id="32f66-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="32f66-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="32f66-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="32f66-133">Response</span></span>
<span data-ttu-id="32f66-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="32f66-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1610

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsPhoneXAP",
      "id": "301ddc77-dc77-301d-77dc-1d3077dc1d30",
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
      "productIdentifier": "Product Identifier value",
      "identityVersion": "Identity Version value"
    }
  ]
}
```




