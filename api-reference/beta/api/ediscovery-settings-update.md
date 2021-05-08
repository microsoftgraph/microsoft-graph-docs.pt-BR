---
title: Atualizar configurações
description: Atualize as propriedades de um objeto settings.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: bbaf760948fc8ee7079e1c746405afddcd73a2b5
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52240823"
---
# <a name="update-settings"></a><span data-ttu-id="b6508-103">Atualizar configurações</span><span class="sxs-lookup"><span data-stu-id="b6508-103">Update settings</span></span>

<span data-ttu-id="b6508-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="b6508-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b6508-105">Atualize as propriedades de [um objeto settings.](../resources/ediscovery-settings.md)</span><span class="sxs-lookup"><span data-stu-id="b6508-105">Update the properties of a [settings](../resources/ediscovery-settings.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b6508-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b6508-106">Permissions</span></span>

<span data-ttu-id="b6508-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6508-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6508-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b6508-109">Permission type</span></span>|<span data-ttu-id="b6508-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b6508-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b6508-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b6508-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b6508-112">eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6508-112">eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="b6508-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b6508-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b6508-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b6508-114">Not supported.</span></span>|
|<span data-ttu-id="b6508-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b6508-115">Application</span></span>|<span data-ttu-id="b6508-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b6508-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b6508-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b6508-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /compliance/ediscovery/cases/{caseId}/settings
```

## <a name="request-headers"></a><span data-ttu-id="b6508-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b6508-118">Request headers</span></span>

|<span data-ttu-id="b6508-119">Nome</span><span class="sxs-lookup"><span data-stu-id="b6508-119">Name</span></span>|<span data-ttu-id="b6508-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="b6508-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b6508-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="b6508-121">Authorization</span></span>|<span data-ttu-id="b6508-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b6508-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="b6508-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b6508-124">Content-Type</span></span>|<span data-ttu-id="b6508-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b6508-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b6508-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b6508-127">Request body</span></span>

<span data-ttu-id="b6508-128">No corpo da solicitação, fornece uma representação JSON do [objeto settings.](../resources/ediscovery-settings.md)</span><span class="sxs-lookup"><span data-stu-id="b6508-128">In the request body, supply a JSON representation of the [settings](../resources/ediscovery-settings.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="b6508-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6508-129">Response</span></span>

<span data-ttu-id="b6508-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b6508-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="b6508-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b6508-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b6508-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b6508-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="b6508-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="b6508-133">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="b6508-134">C#</span><span class="sxs-lookup"><span data-stu-id="b6508-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-settings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b6508-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b6508-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-settings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b6508-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b6508-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-settings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b6508-137">Java</span><span class="sxs-lookup"><span data-stu-id="b6508-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-settings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b6508-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6508-138">Response</span></span>

<span data-ttu-id="b6508-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b6508-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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
