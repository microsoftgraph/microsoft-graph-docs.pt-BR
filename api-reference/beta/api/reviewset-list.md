---
title: Listar reviewSets
description: Recupere a lista de objetos reviewset em um objeto ediscoveryCase.
localization_priority: Normal
author: mahage-msft
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 6fb2c5c1874e9c4fdd6dc59bf4b52783b6e1f88b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48085418"
---
# <a name="list-reviewsets"></a><span data-ttu-id="c4772-103">Listar reviewSets</span><span class="sxs-lookup"><span data-stu-id="c4772-103">List reviewSets</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c4772-104">Recupere a lista de objetos [reviewset](../resources/reviewset.md) em um objeto [ediscoveryCase](../resources/ediscoverycase.md) .</span><span class="sxs-lookup"><span data-stu-id="c4772-104">Retrieve the list of [reviewSet](../resources/reviewset.md) objects in an [ediscoveryCase](../resources/ediscoverycase.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c4772-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="c4772-105">Permissions</span></span>

<span data-ttu-id="c4772-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c4772-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c4772-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c4772-108">Permission type</span></span>                        | <span data-ttu-id="c4772-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c4772-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c4772-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c4772-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="c4772-111">User.Read</span><span class="sxs-lookup"><span data-stu-id="c4772-111">User.Read</span></span> |
| <span data-ttu-id="c4772-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c4772-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c4772-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c4772-113">Not supported.</span></span> |
| <span data-ttu-id="c4772-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c4772-114">Application</span></span>                            | <span data-ttu-id="c4772-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c4772-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c4772-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c4772-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /compliance/ediscovery/cases/{id}/reviewSets
```

## <a name="request-headers"></a><span data-ttu-id="c4772-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c4772-117">Request headers</span></span>

| <span data-ttu-id="c4772-118">Nome</span><span class="sxs-lookup"><span data-stu-id="c4772-118">Name</span></span>          | <span data-ttu-id="c4772-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="c4772-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="c4772-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="c4772-120">Authorization</span></span> | <span data-ttu-id="c4772-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c4772-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c4772-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c4772-123">Request body</span></span>

<span data-ttu-id="c4772-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c4772-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c4772-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4772-125">Response</span></span>

<span data-ttu-id="c4772-126">Se bem-sucedido, este método retorna um `200 OK` código de resposta e a coleção [reviewset](../resources/reviewset.md) solicitada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c4772-126">If successful, this method returns a `200 OK` response code and the requested [reviewSet](../resources/reviewset.md) collection in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c4772-127">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c4772-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c4772-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c4772-128">Request</span></span>

<span data-ttu-id="c4772-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c4772-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c4772-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="c4772-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_reviewset",
  "@odata.type": "microsoft.graph.reviewSet"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/6f65a8e4-c6a0-4cff-8a81-c9ab5df7290d/reviewSets
```
# <a name="c"></a>[<span data-ttu-id="c4772-131">C#</span><span class="sxs-lookup"><span data-stu-id="c4772-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-reviewset-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c4772-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c4772-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-reviewset-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c4772-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c4772-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-reviewset-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c4772-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4772-134">Response</span></span>

<span data-ttu-id="c4772-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c4772-135">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.reviewSet"
} -->

```http
HTTP/1.1 200 OK

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#cases",
    "@odata.nextLink": "https://graph.microsoft.com/beta/compliance/ediscovery/cases?$skiptoken=<encodedPageToken>",
    "value": [
        {
            "id": "f6a91542-4ce7-4712-b275-c29545dd8507",
            "displayName": "My Reviewset 1",
            "createdBy": {
                "user": {
                    "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
                    "displayName": "eDiscovery admin"
                }
            },
            "createdDateTime": "2020-01-16T11:58:27.1408174Z"
        },
        {
            "id": "0d78ec4a-aa91-41ea-8da8-d68b030c168f",
            "displayName": "My Reviewset 2",
            "createdBy": {
                "user": {
                    "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
                    "displayName": "eDiscovery admin"
                }
            },
            "createdDateTime": "2020-01-16T12:03:32.2038960Z"
        }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete reviewSet",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


