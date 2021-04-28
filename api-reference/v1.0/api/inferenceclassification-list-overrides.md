---
title: List overrides
description: Obtenha as substituições que um usuário configurou para sempre classificar as mensagens de determinados remetentes de maneiras específicas.
localization_priority: Normal
author: abheek-das
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: fb6cd4c87c5ee06e0d9849bdaa13e62b616c7d3c
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051372"
---
# <a name="list-overrides"></a><span data-ttu-id="c295b-103">List overrides</span><span class="sxs-lookup"><span data-stu-id="c295b-103">List overrides</span></span>

<span data-ttu-id="c295b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c295b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c295b-105">Obtenha as substituições que um usuário configurou para sempre classificar as mensagens de determinados remetentes de maneiras específicas.</span><span class="sxs-lookup"><span data-stu-id="c295b-105">Get the overrides that a user has set up to always classify messages from certain senders in specific ways.</span></span>

<span data-ttu-id="c295b-p101">Cada substituição corresponde a um endereço SMTP de um remetente. Inicialmente, um usuário não tem quaisquer substituições.</span><span class="sxs-lookup"><span data-stu-id="c295b-p101">Each override corresponds to an SMTP address of a sender. Initially, a user does not have any overrides.</span></span>
## <a name="permissions"></a><span data-ttu-id="c295b-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="c295b-108">Permissions</span></span>
<span data-ttu-id="c295b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c295b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c295b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c295b-111">Permission type</span></span>      | <span data-ttu-id="c295b-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c295b-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c295b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c295b-113">Delegated (work or school account)</span></span> | <span data-ttu-id="c295b-114">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="c295b-114">Mail.Read</span></span>    |
|<span data-ttu-id="c295b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c295b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c295b-116">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="c295b-116">Mail.Read</span></span>    |
|<span data-ttu-id="c295b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c295b-117">Application</span></span> | <span data-ttu-id="c295b-118">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="c295b-118">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="c295b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c295b-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/inferenceClassification/overrides
GET /users/{id}/inferenceClassification/overrides
```

## <a name="request-headers"></a><span data-ttu-id="c295b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c295b-120">Request headers</span></span>
| <span data-ttu-id="c295b-121">Nome</span><span class="sxs-lookup"><span data-stu-id="c295b-121">Name</span></span>       | <span data-ttu-id="c295b-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="c295b-122">Type</span></span> | <span data-ttu-id="c295b-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="c295b-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c295b-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="c295b-124">Authorization</span></span>  | <span data-ttu-id="c295b-125">string</span><span class="sxs-lookup"><span data-stu-id="c295b-125">string</span></span>  | <span data-ttu-id="c295b-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c295b-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c295b-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c295b-128">Request body</span></span>
<span data-ttu-id="c295b-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c295b-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c295b-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="c295b-130">Response</span></span>

<span data-ttu-id="c295b-p104">Se bem sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) no corpo da resposta. Retorna uma coleção vazia se o usuário não tiver quaisquer substituições configuradas.</span><span class="sxs-lookup"><span data-stu-id="c295b-p104">If successful, this method returns a `200 OK` response code and a collection of [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) objects in the response body. An empty collection is returned if the user doesn't have any overrides set up.</span></span>
## <a name="example"></a><span data-ttu-id="c295b-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c295b-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c295b-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c295b-134">Request</span></span>
<span data-ttu-id="c295b-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c295b-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c295b-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="c295b-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_overrides"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/inferenceClassification/overrides
```
# <a name="c"></a>[<span data-ttu-id="c295b-137">C#</span><span class="sxs-lookup"><span data-stu-id="c295b-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-overrides-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c295b-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c295b-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-overrides-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c295b-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c295b-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-overrides-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c295b-140">Java</span><span class="sxs-lookup"><span data-stu-id="c295b-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-overrides-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c295b-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="c295b-141">Response</span></span>
<span data-ttu-id="c295b-142">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c295b-142">Here is an example of the response.</span></span> <span data-ttu-id="c295b-143">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c295b-143">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.inferenceClassificationOverride",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "classifyAs": "focused",
      "senderEmailAddress": {
        "name": "Samantha Booth",
        "address": "samanthab@adatum.onmicrosoft.com"
      },
      "id": "98f5bdef-576a-404d-a2ea-07a3cf11a9b9"
    },
    {
      "classifyAs": "other",
      "senderEmailAddress": {
        "name": "Randi Welch",
        "address": "randiw@adatum.onmicrosoft.com"
      },
      "id": "98f5bdef-576a-404d-a2ea-07a3cf34af4r"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List overrides",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

