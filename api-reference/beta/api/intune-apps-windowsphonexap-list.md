---
title: Lista windowsPhoneXAPs
description: Lista as propriedades e os relacionamentos dos objetos windowsPhoneXAP.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5191340823639d857a6c06f99b53a9ee24c6a1d4
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406672"
---
# <a name="list-windowsphonexaps"></a><span data-ttu-id="0b0c6-103">Lista windowsPhoneXAPs</span><span class="sxs-lookup"><span data-stu-id="0b0c6-103">List windowsPhoneXAPs</span></span>

> <span data-ttu-id="0b0c6-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="0b0c6-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0b0c6-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="0b0c6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0b0c6-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="0b0c6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0b0c6-107">Lista as propriedades e os relacionamentos dos objetos [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) .</span><span class="sxs-lookup"><span data-stu-id="0b0c6-107">List properties and relationships of the [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0b0c6-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0b0c6-108">Prerequisites</span></span>
<span data-ttu-id="0b0c6-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="0b0c6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="0b0c6-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0b0c6-111">Permission type</span></span>|<span data-ttu-id="0b0c6-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0b0c6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0b0c6-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0b0c6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0b0c6-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="0b0c6-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="0b0c6-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0b0c6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0b0c6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0b0c6-116">Not supported.</span></span>|
|<span data-ttu-id="0b0c6-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0b0c6-117">Application</span></span>|<span data-ttu-id="0b0c6-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0b0c6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0b0c6-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0b0c6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="0b0c6-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0b0c6-120">Request headers</span></span>
|<span data-ttu-id="0b0c6-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0b0c6-121">Header</span></span>|<span data-ttu-id="0b0c6-122">Valor</span><span class="sxs-lookup"><span data-stu-id="0b0c6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0b0c6-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0b0c6-123">Authorization</span></span>|<span data-ttu-id="0b0c6-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0b0c6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0b0c6-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0b0c6-125">Accept</span></span>|<span data-ttu-id="0b0c6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0b0c6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0b0c6-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0b0c6-127">Request body</span></span>
<span data-ttu-id="0b0c6-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0b0c6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0b0c6-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="0b0c6-129">Response</span></span>
<span data-ttu-id="0b0c6-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0b0c6-130">If successful, this method returns a `200 OK` response code and a collection of [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0b0c6-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0b0c6-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="0b0c6-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0b0c6-132">Request</span></span>
<span data-ttu-id="0b0c6-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0b0c6-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="0b0c6-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="0b0c6-134">Response</span></span>
<span data-ttu-id="0b0c6-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0b0c6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1525

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
        "v10_1803": true
      },
      "productIdentifier": "Product Identifier value",
      "identityVersion": "Identity Version value"
    }
  ]
}
```




