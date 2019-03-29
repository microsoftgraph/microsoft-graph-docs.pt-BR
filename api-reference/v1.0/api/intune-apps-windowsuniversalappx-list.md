---
title: Listar windowsUniversalAppXs
description: Listar propriedades e relações dos objetos windowsUniversalAppX.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a7018bf105e166f7b796a2bf3a12dfeca844daac
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30964609"
---
# <a name="list-windowsuniversalappxs"></a><span data-ttu-id="5ff7f-103">Listar windowsUniversalAppXs</span><span class="sxs-lookup"><span data-stu-id="5ff7f-103">List windowsUniversalAppXs</span></span>

> <span data-ttu-id="5ff7f-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5ff7f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5ff7f-105">Listar propriedades e relações dos objetos [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md).</span><span class="sxs-lookup"><span data-stu-id="5ff7f-105">List properties and relationships of the [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5ff7f-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5ff7f-106">Prerequisites</span></span>
<span data-ttu-id="5ff7f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5ff7f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ff7f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5ff7f-109">Permission type</span></span>|<span data-ttu-id="5ff7f-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5ff7f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5ff7f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5ff7f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5ff7f-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="5ff7f-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="5ff7f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5ff7f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5ff7f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5ff7f-114">Not supported.</span></span>|
|<span data-ttu-id="5ff7f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5ff7f-115">Application</span></span>|<span data-ttu-id="5ff7f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5ff7f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5ff7f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5ff7f-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="5ff7f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5ff7f-118">Request headers</span></span>
|<span data-ttu-id="5ff7f-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5ff7f-119">Header</span></span>|<span data-ttu-id="5ff7f-120">Valor</span><span class="sxs-lookup"><span data-stu-id="5ff7f-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5ff7f-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="5ff7f-121">Authorization</span></span>|<span data-ttu-id="5ff7f-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5ff7f-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5ff7f-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5ff7f-123">Accept</span></span>|<span data-ttu-id="5ff7f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="5ff7f-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5ff7f-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5ff7f-125">Request body</span></span>
<span data-ttu-id="5ff7f-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5ff7f-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5ff7f-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ff7f-127">Response</span></span>
<span data-ttu-id="5ff7f-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5ff7f-128">If successful, this method returns a `200 OK` response code and a collection of [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5ff7f-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5ff7f-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="5ff7f-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5ff7f-130">Request</span></span>
<span data-ttu-id="5ff7f-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5ff7f-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="5ff7f-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ff7f-132">Response</span></span>
<span data-ttu-id="5ff7f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5ff7f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1534

{
  "value": [
    {
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
      "publishingState": "processing",
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
        "v10_0": true
      },
      "identityVersion": "Identity Version value"
    }
  ]
}
```



