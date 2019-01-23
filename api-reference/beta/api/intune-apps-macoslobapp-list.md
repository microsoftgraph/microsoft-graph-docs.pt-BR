---
title: Lista macOSLobApps
description: Lista as propriedades e os relacionamentos dos objetos macOSLobApp.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 073d3e529c7dba13f086085c23997945e8a28a4f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29409493"
---
# <a name="list-macoslobapps"></a><span data-ttu-id="c91d8-103">Lista macOSLobApps</span><span class="sxs-lookup"><span data-stu-id="c91d8-103">List macOSLobApps</span></span>

> <span data-ttu-id="c91d8-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="c91d8-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c91d8-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c91d8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c91d8-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="c91d8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c91d8-107">Lista as propriedades e os relacionamentos dos objetos [macOSLobApp](../resources/intune-apps-macoslobapp.md) .</span><span class="sxs-lookup"><span data-stu-id="c91d8-107">List properties and relationships of the [macOSLobApp](../resources/intune-apps-macoslobapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c91d8-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c91d8-108">Prerequisites</span></span>
<span data-ttu-id="c91d8-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c91d8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c91d8-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c91d8-111">Permission type</span></span>|<span data-ttu-id="c91d8-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c91d8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c91d8-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c91d8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c91d8-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c91d8-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="c91d8-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c91d8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c91d8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c91d8-116">Not supported.</span></span>|
|<span data-ttu-id="c91d8-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c91d8-117">Application</span></span>|<span data-ttu-id="c91d8-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c91d8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c91d8-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c91d8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="c91d8-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c91d8-120">Request headers</span></span>
|<span data-ttu-id="c91d8-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c91d8-121">Header</span></span>|<span data-ttu-id="c91d8-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c91d8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c91d8-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c91d8-123">Authorization</span></span>|<span data-ttu-id="c91d8-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c91d8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c91d8-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c91d8-125">Accept</span></span>|<span data-ttu-id="c91d8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c91d8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c91d8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c91d8-127">Request body</span></span>
<span data-ttu-id="c91d8-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c91d8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c91d8-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="c91d8-129">Response</span></span>
<span data-ttu-id="c91d8-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [macOSLobApp](../resources/intune-apps-macoslobapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c91d8-130">If successful, this method returns a `200 OK` response code and a collection of [macOSLobApp](../resources/intune-apps-macoslobapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c91d8-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c91d8-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="c91d8-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c91d8-132">Request</span></span>
<span data-ttu-id="c91d8-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c91d8-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="c91d8-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="c91d8-134">Response</span></span>
<span data-ttu-id="c91d8-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c91d8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1968

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.macOSLobApp",
      "id": "7be9250a-250a-7be9-0a25-e97b0a25e97b",
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
      "minimumSupportedOperatingSystem": {
        "@odata.type": "microsoft.graph.macOSMinimumOperatingSystem",
        "v10_7": true,
        "v10_8": true,
        "v10_9": true,
        "v10_10": true,
        "v10_11": true,
        "v10_12": true,
        "v10_13": true
      },
      "buildNumber": "Build Number value",
      "versionNumber": "Version Number value",
      "childApps": [
        {
          "@odata.type": "microsoft.graph.macOSLobChildApp",
          "bundleId": "Bundle Id value",
          "buildNumber": "Build Number value",
          "versionNumber": "Version Number value"
        }
      ],
      "identityVersion": "Identity Version value",
      "md5HashChunkSize": 0,
      "md5Hash": [
        "Md5Hash value"
      ],
      "ignoreVersionDetection": true
    }
  ]
}
```




