---
title: Listar windowsQualityUpdateCatalogItems
description: Listar propriedades e relações dos objetos windowsQualityUpdateCatalogItem.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d97c24f7e216145ed9862e7117cbb074d8b1fbb9
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160170"
---
# <a name="list-windowsqualityupdatecatalogitems"></a><span data-ttu-id="89e35-103">Listar windowsQualityUpdateCatalogItems</span><span class="sxs-lookup"><span data-stu-id="89e35-103">List windowsQualityUpdateCatalogItems</span></span>

<span data-ttu-id="89e35-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="89e35-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="89e35-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="89e35-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="89e35-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="89e35-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="89e35-107">Listar propriedades e relações dos [objetos windowsQualityUpdateCatalogItem.](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md)</span><span class="sxs-lookup"><span data-stu-id="89e35-107">List properties and relationships of the [windowsQualityUpdateCatalogItem](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="89e35-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="89e35-108">Prerequisites</span></span>
<span data-ttu-id="89e35-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="89e35-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89e35-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="89e35-111">Permission type</span></span>|<span data-ttu-id="89e35-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="89e35-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="89e35-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="89e35-113">Delegated (work or school account)</span></span>|<span data-ttu-id="89e35-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="89e35-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="89e35-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="89e35-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="89e35-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="89e35-116">Not supported.</span></span>|
|<span data-ttu-id="89e35-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="89e35-117">Application</span></span>|<span data-ttu-id="89e35-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="89e35-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="89e35-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="89e35-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsUpdateCatalogItems
```

## <a name="request-headers"></a><span data-ttu-id="89e35-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="89e35-120">Request headers</span></span>
|<span data-ttu-id="89e35-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="89e35-121">Header</span></span>|<span data-ttu-id="89e35-122">Valor</span><span class="sxs-lookup"><span data-stu-id="89e35-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="89e35-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="89e35-123">Authorization</span></span>|<span data-ttu-id="89e35-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="89e35-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="89e35-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="89e35-125">Accept</span></span>|<span data-ttu-id="89e35-126">application/json</span><span class="sxs-lookup"><span data-stu-id="89e35-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="89e35-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="89e35-127">Request body</span></span>
<span data-ttu-id="89e35-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="89e35-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="89e35-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="89e35-129">Response</span></span>
<span data-ttu-id="89e35-130">Se bem-sucedido, este método retorna um código de resposta e uma coleção de `200 OK` [objetos windowsQualityUpdateCatalogItem](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="89e35-130">If successful, this method returns a `200 OK` response code and a collection of [windowsQualityUpdateCatalogItem](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="89e35-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="89e35-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="89e35-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="89e35-132">Request</span></span>
<span data-ttu-id="89e35-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="89e35-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsUpdateCatalogItems
```

### <a name="response"></a><span data-ttu-id="89e35-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="89e35-134">Response</span></span>
<span data-ttu-id="89e35-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="89e35-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 382

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsQualityUpdateCatalogItem",
      "id": "8eb831ba-31ba-8eb8-ba31-b88eba31b88e",
      "displayName": "Display Name value",
      "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
      "kbArticleId": "Kb Article Id value",
      "classification": "security",
      "isExpeditable": true
    }
  ]
}
```




