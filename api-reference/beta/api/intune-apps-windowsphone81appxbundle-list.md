---
title: Listar windowsPhone81AppXBundles
description: Listar Propriedades e relações dos objetos windowsPhone81AppXBundle.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e4581c307b37c765218b921ded91264d0cc88263
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35959933"
---
# <a name="list-windowsphone81appxbundles"></a><span data-ttu-id="84434-103">Listar windowsPhone81AppXBundles</span><span class="sxs-lookup"><span data-stu-id="84434-103">List windowsPhone81AppXBundles</span></span>

> <span data-ttu-id="84434-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="84434-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="84434-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="84434-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="84434-106">Listar Propriedades e relações dos objetos [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) .</span><span class="sxs-lookup"><span data-stu-id="84434-106">List properties and relationships of the [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="84434-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="84434-107">Prerequisites</span></span>
<span data-ttu-id="84434-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="84434-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="84434-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="84434-110">Permission type</span></span>|<span data-ttu-id="84434-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="84434-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="84434-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="84434-112">Delegated (work or school account)</span></span>|<span data-ttu-id="84434-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="84434-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="84434-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="84434-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="84434-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="84434-115">Not supported.</span></span>|
|<span data-ttu-id="84434-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="84434-116">Application</span></span>|<span data-ttu-id="84434-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="84434-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="84434-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="84434-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="84434-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="84434-119">Request headers</span></span>
|<span data-ttu-id="84434-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="84434-120">Header</span></span>|<span data-ttu-id="84434-121">Valor</span><span class="sxs-lookup"><span data-stu-id="84434-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="84434-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="84434-122">Authorization</span></span>|<span data-ttu-id="84434-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="84434-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="84434-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="84434-124">Accept</span></span>|<span data-ttu-id="84434-125">application/json</span><span class="sxs-lookup"><span data-stu-id="84434-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="84434-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="84434-126">Request body</span></span>
<span data-ttu-id="84434-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="84434-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="84434-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="84434-128">Response</span></span>
<span data-ttu-id="84434-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="84434-129">If successful, this method returns a `200 OK` response code and a collection of [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="84434-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="84434-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="84434-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="84434-131">Request</span></span>
<span data-ttu-id="84434-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="84434-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="84434-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="84434-133">Response</span></span>
<span data-ttu-id="84434-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="84434-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2796

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsPhone81AppXBundle",
      "id": "2433be7c-be7c-2433-7cbe-33247cbe3324",
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
      "identityVersion": "Identity Version value",
      "appXPackageInformationList": [
        {
          "@odata.type": "microsoft.graph.windowsPackageInformation",
          "applicableArchitecture": "x86",
          "displayName": "Display Name value",
          "identityName": "Identity Name value",
          "identityPublisher": "Identity Publisher value",
          "identityResourceIdentifier": "Identity Resource Identifier value",
          "identityVersion": "Identity Version value",
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
          }
        }
      ]
    }
  ]
}
```





