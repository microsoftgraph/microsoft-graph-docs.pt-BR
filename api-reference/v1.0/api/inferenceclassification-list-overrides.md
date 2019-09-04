---
title: Substituições de lista
description: Obtenha as substituições que um usuário configurou para sempre classificar as mensagens de determinados remetentes de maneiras específicas.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: c391cdc967a65a1371a9c0a6c27c002c0b06749a
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36726743"
---
# <a name="list-overrides"></a><span data-ttu-id="1bd7b-103">Substituições de lista</span><span class="sxs-lookup"><span data-stu-id="1bd7b-103">List overrides</span></span>

<span data-ttu-id="1bd7b-104">Obtenha as substituições que um usuário configurou para sempre classificar as mensagens de determinados remetentes de maneiras específicas.</span><span class="sxs-lookup"><span data-stu-id="1bd7b-104">Get the overrides that a user has set up to always classify messages from certain senders in specific ways.</span></span>

<span data-ttu-id="1bd7b-p101">Cada substituição corresponde a um endereço SMTP de um remetente. Inicialmente, um usuário não tem quaisquer substituições.</span><span class="sxs-lookup"><span data-stu-id="1bd7b-p101">Each override corresponds to an SMTP address of a sender. Initially, a user does not have any overrides.</span></span>
## <a name="permissions"></a><span data-ttu-id="1bd7b-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="1bd7b-107">Permissions</span></span>
<span data-ttu-id="1bd7b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1bd7b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1bd7b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1bd7b-110">Permission type</span></span>      | <span data-ttu-id="1bd7b-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1bd7b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1bd7b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1bd7b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1bd7b-113">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="1bd7b-113">Mail.Read</span></span>    |
|<span data-ttu-id="1bd7b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1bd7b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1bd7b-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="1bd7b-115">Mail.Read</span></span>    |
|<span data-ttu-id="1bd7b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1bd7b-116">Application</span></span> | <span data-ttu-id="1bd7b-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="1bd7b-117">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="1bd7b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1bd7b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/inferenceClassification/overrides
GET /users/{id}/inferenceClassification/overrides
```

## <a name="request-headers"></a><span data-ttu-id="1bd7b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1bd7b-119">Request headers</span></span>
| <span data-ttu-id="1bd7b-120">Nome</span><span class="sxs-lookup"><span data-stu-id="1bd7b-120">Name</span></span>       | <span data-ttu-id="1bd7b-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="1bd7b-121">Type</span></span> | <span data-ttu-id="1bd7b-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="1bd7b-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1bd7b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1bd7b-123">Authorization</span></span>  | <span data-ttu-id="1bd7b-124">string</span><span class="sxs-lookup"><span data-stu-id="1bd7b-124">string</span></span>  | <span data-ttu-id="1bd7b-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1bd7b-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1bd7b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1bd7b-127">Request body</span></span>
<span data-ttu-id="1bd7b-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1bd7b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1bd7b-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="1bd7b-129">Response</span></span>

<span data-ttu-id="1bd7b-p104">Se bem sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) no corpo da resposta. Retorna uma coleção vazia se o usuário não tiver quaisquer substituições configuradas.</span><span class="sxs-lookup"><span data-stu-id="1bd7b-p104">If successful, this method returns a `200 OK` response code and a collection of [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) objects in the response body. An empty collection is returned if the user doesn't have any overrides set up.</span></span>
## <a name="example"></a><span data-ttu-id="1bd7b-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1bd7b-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1bd7b-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1bd7b-133">Request</span></span>
<span data-ttu-id="1bd7b-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1bd7b-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1bd7b-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="1bd7b-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_overrides"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/inferenceClassification/overrides
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1bd7b-136">C#</span><span class="sxs-lookup"><span data-stu-id="1bd7b-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-overrides-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1bd7b-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1bd7b-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-overrides-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1bd7b-138">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="1bd7b-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-overrides-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="1bd7b-139">Java</span><span class="sxs-lookup"><span data-stu-id="1bd7b-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-overrides-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="1bd7b-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="1bd7b-140">Response</span></span>
<span data-ttu-id="1bd7b-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1bd7b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
