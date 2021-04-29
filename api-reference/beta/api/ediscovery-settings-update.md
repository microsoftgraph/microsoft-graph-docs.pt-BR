---
title: Atualizar configurações
description: Atualize as propriedades de um objeto settings.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 2892e2ecb3d0eea720267f9cc8ea5ae635bdb303
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/29/2021
ms.locfileid: "52080692"
---
# <a name="update-settings"></a><span data-ttu-id="e40b4-103">Atualizar configurações</span><span class="sxs-lookup"><span data-stu-id="e40b4-103">Update settings</span></span>

<span data-ttu-id="e40b4-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="e40b4-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e40b4-105">Atualize as propriedades de [um objeto settings.](../resources/ediscovery-settings.md)</span><span class="sxs-lookup"><span data-stu-id="e40b4-105">Update the properties of a [settings](../resources/ediscovery-settings.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e40b4-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e40b4-106">Permissions</span></span>

<span data-ttu-id="e40b4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e40b4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e40b4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e40b4-109">Permission type</span></span>|<span data-ttu-id="e40b4-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e40b4-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e40b4-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e40b4-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e40b4-112">eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e40b4-112">eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="e40b4-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e40b4-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e40b4-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e40b4-114">Not supported.</span></span>|
|<span data-ttu-id="e40b4-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e40b4-115">Application</span></span>|<span data-ttu-id="e40b4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e40b4-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e40b4-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e40b4-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /compliance/ediscovery/cases/{caseId}/settings
```

## <a name="request-headers"></a><span data-ttu-id="e40b4-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e40b4-118">Request headers</span></span>

|<span data-ttu-id="e40b4-119">Nome</span><span class="sxs-lookup"><span data-stu-id="e40b4-119">Name</span></span>|<span data-ttu-id="e40b4-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="e40b4-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e40b4-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="e40b4-121">Authorization</span></span>|<span data-ttu-id="e40b4-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e40b4-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="e40b4-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e40b4-124">Content-Type</span></span>|<span data-ttu-id="e40b4-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e40b4-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e40b4-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e40b4-127">Request body</span></span>

<span data-ttu-id="e40b4-128">No corpo da solicitação, fornece uma representação JSON do [objeto settings.](../resources/ediscovery-settings.md)</span><span class="sxs-lookup"><span data-stu-id="e40b4-128">In the request body, supply a JSON representation of the [settings](../resources/ediscovery-settings.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e40b4-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="e40b4-129">Response</span></span>

<span data-ttu-id="e40b4-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e40b4-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="e40b4-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e40b4-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e40b4-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e40b4-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_settings"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/compliance/ediscovery/cases/{caseId}/settings
Content-Type: application/json
Content-length: 350

{
    "redundancyDetection": {
        "isEnabled": false,
        "similarityThreshold": 70,
        "minWords": 12,
        "maxWords": 400000
    },
    "topicModeling": {
        "isEnabled": false,
        "ignoreNumbers": false,
        "topicCount": 50,
        "dynamicallyAdjustTopicCount": false
    },
    "ocr": {
        "isEnabled": true,
        "maxImageSize": 12000
    }
}
```

### <a name="response"></a><span data-ttu-id="e40b4-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="e40b4-133">Response</span></span>

<span data-ttu-id="e40b4-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e40b4-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
cache-control: no-cache
client-request-id: e9fc7554-ca5e-0928-fc09-9c5825820c88
content-length: 0
request-id: 1f53bd55-f099-46cb-91df-8f5d466aba3a
```
