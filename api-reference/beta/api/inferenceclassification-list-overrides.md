---
title: List overrides
description: Obtenha as substituições da Caixa de Entrada Destaques que um usuário configurou para sempre classificar as mensagens de determinados remetentes de maneiras específicas.
localization_priority: Normal
doc_type: apiPageType
author: abheek-das
ms.prod: ''
ms.openlocfilehash: 07de9e0bb9d8992811b64a8fe19685a2a329a8c1
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52040606"
---
# <a name="list-overrides"></a><span data-ttu-id="c2368-103">List overrides</span><span class="sxs-lookup"><span data-stu-id="c2368-103">List overrides</span></span>

<span data-ttu-id="c2368-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c2368-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c2368-105">Obter as [substituições da Caixa de Entrada Focalizadas](../resources/manage-focused-inbox.md) que um usuário definiu para sempre classificar mensagens de determinados envios de maneiras específicas.</span><span class="sxs-lookup"><span data-stu-id="c2368-105">Get the [Focused Inbox](../resources/manage-focused-inbox.md) overrides that a user has set up to always classify messages from certain senders in specific ways.</span></span>

<span data-ttu-id="c2368-p101">Cada substituição corresponde a um endereço SMTP de um remetente. Inicialmente, um usuário não tem quaisquer substituições.</span><span class="sxs-lookup"><span data-stu-id="c2368-p101">Each override corresponds to an SMTP address of a sender. Initially, a user does not have any overrides.</span></span>
## <a name="permissions"></a><span data-ttu-id="c2368-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="c2368-108">Permissions</span></span>
<span data-ttu-id="c2368-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c2368-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c2368-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c2368-111">Permission type</span></span>      | <span data-ttu-id="c2368-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c2368-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c2368-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c2368-113">Delegated (work or school account)</span></span> | <span data-ttu-id="c2368-114">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="c2368-114">Mail.Read</span></span>    |
|<span data-ttu-id="c2368-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c2368-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c2368-116">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="c2368-116">Mail.Read</span></span>    |
|<span data-ttu-id="c2368-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c2368-117">Application</span></span> | <span data-ttu-id="c2368-118">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="c2368-118">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="c2368-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c2368-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/inferenceClassification/overrides
GET /users/{id}/inferenceClassification/overrides
```

## <a name="request-headers"></a><span data-ttu-id="c2368-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c2368-120">Request headers</span></span>
| <span data-ttu-id="c2368-121">Nome</span><span class="sxs-lookup"><span data-stu-id="c2368-121">Name</span></span>       | <span data-ttu-id="c2368-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="c2368-122">Type</span></span> | <span data-ttu-id="c2368-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="c2368-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c2368-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="c2368-124">Authorization</span></span>  | <span data-ttu-id="c2368-125">string</span><span class="sxs-lookup"><span data-stu-id="c2368-125">string</span></span>  | <span data-ttu-id="c2368-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c2368-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c2368-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c2368-128">Request body</span></span>
<span data-ttu-id="c2368-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c2368-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c2368-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="c2368-130">Response</span></span>

<span data-ttu-id="c2368-131">Se bem sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c2368-131">If successful, this method returns a `200 OK` response code and a collection of [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c2368-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c2368-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c2368-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c2368-133">Request</span></span>
<span data-ttu-id="c2368-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c2368-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c2368-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="c2368-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_overrides"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/inferenceClassification/overrides
```
# <a name="c"></a>[<span data-ttu-id="c2368-136">C#</span><span class="sxs-lookup"><span data-stu-id="c2368-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-overrides-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c2368-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c2368-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-overrides-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c2368-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c2368-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-overrides-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c2368-139">Java</span><span class="sxs-lookup"><span data-stu-id="c2368-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-overrides-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c2368-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="c2368-140">Response</span></span>
<span data-ttu-id="c2368-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c2368-141">Here is an example of the response.</span></span> <span data-ttu-id="c2368-142">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c2368-142">Note: The response object shown here might be shortened for readability.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List overrides",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


