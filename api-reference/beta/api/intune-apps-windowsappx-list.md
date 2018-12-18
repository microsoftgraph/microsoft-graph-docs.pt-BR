---
title: Lista windowsAppXs
description: Lista as propriedades e os relacionamentos dos objetos windowsAppX.
author: tfitzmac
ms.openlocfilehash: 8c951182c4e3be25d0e418d118c2e4a6a3b1c2a8
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27355458"
---
# <a name="list-windowsappxs"></a><span data-ttu-id="70382-103">Lista windowsAppXs</span><span class="sxs-lookup"><span data-stu-id="70382-103">List windowsAppXs</span></span>

> <span data-ttu-id="70382-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="70382-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="70382-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="70382-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="70382-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="70382-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="70382-107">Lista as propriedades e os relacionamentos dos objetos [windowsAppX](../resources/intune-apps-windowsappx.md) .</span><span class="sxs-lookup"><span data-stu-id="70382-107">List properties and relationships of the [windowsAppX](../resources/intune-apps-windowsappx.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="70382-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="70382-108">Prerequisites</span></span>
<span data-ttu-id="70382-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="70382-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="70382-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="70382-111">Permission type</span></span>|<span data-ttu-id="70382-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="70382-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="70382-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="70382-113">Delegated (work or school account)</span></span>|<span data-ttu-id="70382-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="70382-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="70382-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="70382-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="70382-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="70382-116">Not supported.</span></span>|
|<span data-ttu-id="70382-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="70382-117">Application</span></span>|<span data-ttu-id="70382-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="70382-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="70382-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="70382-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="70382-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="70382-120">Request headers</span></span>
|<span data-ttu-id="70382-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="70382-121">Header</span></span>|<span data-ttu-id="70382-122">Valor</span><span class="sxs-lookup"><span data-stu-id="70382-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="70382-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="70382-123">Authorization</span></span>|<span data-ttu-id="70382-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="70382-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="70382-125">Accept</span><span class="sxs-lookup"><span data-stu-id="70382-125">Accept</span></span>|<span data-ttu-id="70382-126">application/json</span><span class="sxs-lookup"><span data-stu-id="70382-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="70382-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="70382-127">Request body</span></span>
<span data-ttu-id="70382-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="70382-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="70382-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="70382-129">Response</span></span>
<span data-ttu-id="70382-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [windowsAppX](../resources/intune-apps-windowsappx.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="70382-130">If successful, this method returns a `200 OK` response code and a collection of [windowsAppX](../resources/intune-apps-windowsappx.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="70382-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="70382-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="70382-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="70382-132">Request</span></span>
<span data-ttu-id="70382-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="70382-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="70382-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="70382-134">Response</span></span>
<span data-ttu-id="70382-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="70382-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1616

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsAppX",
      "id": "b5179a93-9a93-b517-939a-17b5939a17b5",
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
      "committedContentVersion": "Committed Content Version value",
      "fileName": "File Name value",
      "size": 4,
      "applicableArchitectures": "x86",
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
        "v10_1803": true
      },
      "identityVersion": "Identity Version value"
    }
  ]
}
```





