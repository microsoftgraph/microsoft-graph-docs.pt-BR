---
title: Substituições de lista
description: Obtenha as substituições de caixa de entrada destaques que um usuário configurou para sempre classificar as mensagens de determinados remetentes de maneiras específicas.
localization_priority: Normal
doc_type: apiPageType
author: ''
ms.prod: ''
ms.openlocfilehash: 6ecf9cd37015f5472a744dda3c3e4216e55d1cdf
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36419962"
---
# <a name="list-overrides"></a><span data-ttu-id="963df-103">Substituições de lista</span><span class="sxs-lookup"><span data-stu-id="963df-103">List overrides</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="963df-104">Obtenha as substituições de [caixa de entrada destaques](../resources/manage-focused-inbox.md) que um usuário configurou para sempre classificar as mensagens de determinados remetentes de maneiras específicas.</span><span class="sxs-lookup"><span data-stu-id="963df-104">Get the [Focused Inbox](../resources/manage-focused-inbox.md) overrides that a user has set up to always classify messages from certain senders in specific ways.</span></span>

<span data-ttu-id="963df-105">Cada substituição corresponde a um endereço SMTP de um remetente.</span><span class="sxs-lookup"><span data-stu-id="963df-105">Each override corresponds to an SMTP address of a sender.</span></span> <span data-ttu-id="963df-106">Inicialmente, um usuário não tem quaisquer substituições.</span><span class="sxs-lookup"><span data-stu-id="963df-106">Initially, a user does not have any overrides.</span></span>
## <a name="permissions"></a><span data-ttu-id="963df-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="963df-107">Permissions</span></span>
<span data-ttu-id="963df-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="963df-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="963df-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="963df-110">Permission type</span></span>      | <span data-ttu-id="963df-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="963df-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="963df-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="963df-112">Delegated (work or school account)</span></span> | <span data-ttu-id="963df-113">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="963df-113">Mail.Read</span></span>    |
|<span data-ttu-id="963df-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="963df-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="963df-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="963df-115">Mail.Read</span></span>    |
|<span data-ttu-id="963df-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="963df-116">Application</span></span> | <span data-ttu-id="963df-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="963df-117">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="963df-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="963df-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/inferenceClassification/overrides
GET /users/{id}/inferenceClassification/overrides
```

## <a name="request-headers"></a><span data-ttu-id="963df-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="963df-119">Request headers</span></span>
| <span data-ttu-id="963df-120">Nome</span><span class="sxs-lookup"><span data-stu-id="963df-120">Name</span></span>       | <span data-ttu-id="963df-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="963df-121">Type</span></span> | <span data-ttu-id="963df-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="963df-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="963df-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="963df-123">Authorization</span></span>  | <span data-ttu-id="963df-124">string</span><span class="sxs-lookup"><span data-stu-id="963df-124">string</span></span>  | <span data-ttu-id="963df-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="963df-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="963df-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="963df-127">Request body</span></span>
<span data-ttu-id="963df-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="963df-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="963df-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="963df-129">Response</span></span>

<span data-ttu-id="963df-130">Se bem sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="963df-130">If successful, this method returns a `200 OK` response code and a collection of [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="963df-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="963df-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="963df-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="963df-132">Request</span></span>
<span data-ttu-id="963df-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="963df-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="963df-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="963df-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_overrides"
}-->
```http
GET https://graph.microsoft.com/beta/me/inferenceClassification/overrides
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="963df-135">C#</span><span class="sxs-lookup"><span data-stu-id="963df-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-overrides-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="963df-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="963df-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-overrides-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="963df-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="963df-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-overrides-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="963df-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="963df-138">Response</span></span>
<span data-ttu-id="963df-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="963df-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
