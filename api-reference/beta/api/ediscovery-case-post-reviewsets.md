---
title: Criar reviewSet
description: Crie um conjunto de revisão de Descobertas EDiscovery.
localization_priority: Normal
author: mahage-msft
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: ef13c35d3450cfd7f409a59a543662ffeb5db0e5
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52044729"
---
# <a name="create-reviewset"></a><span data-ttu-id="27790-103">Criar reviewSet</span><span class="sxs-lookup"><span data-stu-id="27790-103">Create reviewSet</span></span>

<span data-ttu-id="27790-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="27790-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="27790-105">Crie um novo [objeto reviewSet.](../resources/ediscovery-reviewset.md)</span><span class="sxs-lookup"><span data-stu-id="27790-105">Create a new [reviewSet](../resources/ediscovery-reviewset.md) object.</span></span> <span data-ttu-id="27790-106">O corpo da solicitação contém o nome de exibição do conjunto de revisão, que é a única propriedade writable.</span><span class="sxs-lookup"><span data-stu-id="27790-106">The request body contains the display name of the review set, which is the only writable property.</span></span>

## <a name="permissions"></a><span data-ttu-id="27790-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="27790-107">Permissions</span></span>

<span data-ttu-id="27790-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="27790-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="27790-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="27790-110">Permission type</span></span>|<span data-ttu-id="27790-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="27790-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="27790-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="27790-112">Delegated (work or school account)</span></span>|<span data-ttu-id="27790-113">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27790-113">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="27790-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="27790-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="27790-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="27790-115">Not supported.</span></span>|
|<span data-ttu-id="27790-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="27790-116">Application</span></span>|<span data-ttu-id="27790-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="27790-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="27790-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="27790-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /compliance/ediscovery/cases/{id}/reviewSets
```

## <a name="request-headers"></a><span data-ttu-id="27790-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="27790-119">Request headers</span></span>

| <span data-ttu-id="27790-120">Nome</span><span class="sxs-lookup"><span data-stu-id="27790-120">Name</span></span>       | <span data-ttu-id="27790-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="27790-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="27790-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="27790-122">Authorization</span></span> | <span data-ttu-id="27790-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="27790-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="27790-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="27790-125">Request body</span></span>

<span data-ttu-id="27790-126">No corpo da solicitação, fornece representação JSON do [reviewSet](../resources/ediscovery-reviewset.md).</span><span class="sxs-lookup"><span data-stu-id="27790-126">In the request body, supply JSON representation of the [reviewSet](../resources/ediscovery-reviewset.md).</span></span>  <span data-ttu-id="27790-127">A tabela a seguir lista as propriedades necessárias.</span><span class="sxs-lookup"><span data-stu-id="27790-127">The following table lists the required properties.</span></span>

| <span data-ttu-id="27790-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="27790-128">Property</span></span>     | <span data-ttu-id="27790-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="27790-129">Type</span></span>        | <span data-ttu-id="27790-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="27790-130">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="27790-131">displayName</span><span class="sxs-lookup"><span data-stu-id="27790-131">displayName</span></span>  | <span data-ttu-id="27790-132">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="27790-132">string</span></span>      | <span data-ttu-id="27790-133">O nome do conjunto de revisão.</span><span class="sxs-lookup"><span data-stu-id="27790-133">The name of the review set.</span></span> |

## <a name="response"></a><span data-ttu-id="27790-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="27790-134">Response</span></span>

<span data-ttu-id="27790-135">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto microsoft.graph.ediscovery.reviewSet](../resources/ediscovery-reviewset.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="27790-135">If successful, this method returns a `201 Created` response code and a [microsoft.graph.ediscovery.reviewSet](../resources/ediscovery-reviewset.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="27790-136">Exemplos</span><span class="sxs-lookup"><span data-stu-id="27790-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="27790-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="27790-137">Request</span></span>

<span data-ttu-id="27790-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="27790-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="27790-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="27790-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_reviewset"
}-->

```http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/6f65a8e4-c6a0-4cff-8a81-c9ab5df7290d/reviewSets
Content-type: application/json

{
  "displayName": "My Reviewset 3",
}
```
# <a name="c"></a>[<span data-ttu-id="27790-140">C#</span><span class="sxs-lookup"><span data-stu-id="27790-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-reviewset-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="27790-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="27790-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-reviewset-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="27790-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="27790-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-reviewset-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="27790-143">Java</span><span class="sxs-lookup"><span data-stu-id="27790-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-reviewset-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="27790-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="27790-144">Response</span></span>

<span data-ttu-id="27790-145">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="27790-145">The following is an example of the response.</span></span>

> <span data-ttu-id="27790-146">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="27790-146">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.reviewSet"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/compliance/ediscovery/$metadata#cases('6f65a8e4-c6a0-4cff-8a81-c9ab5df7290d')/reviewSets/$entity",
    "id": "0157910c-57ce-4e48-bd4b-90f3c88ca32e",
    "displayName": "My Reviewset 3",
    "createdBy": {
        "user": {
            "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
            "displayName": "eDiscovery admin"
        }
    },
    "createdDateTime": "2020-03-11T08:40:14.9486058Z"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update reviewset",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


