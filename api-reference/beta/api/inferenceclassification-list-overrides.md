---
title: List overrides
description: Obtenha as substituições da Caixa de Entrada Destaques que um usuário configurou para sempre classificar as mensagens de determinados remetentes de maneiras específicas.
localization_priority: Normal
doc_type: apiPageType
author: ''
ms.prod: ''
ms.openlocfilehash: da22fcbc47a57d07b25b4d937fac3a6d266d9e79
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446426"
---
# <a name="list-overrides"></a><span data-ttu-id="3a4ba-103">List overrides</span><span class="sxs-lookup"><span data-stu-id="3a4ba-103">List overrides</span></span>

<span data-ttu-id="3a4ba-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3a4ba-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3a4ba-105">Obtenha as substituições de [caixa de entrada destaques](../resources/manage-focused-inbox.md) que um usuário configurou para sempre classificar as mensagens de determinados remetentes de maneiras específicas.</span><span class="sxs-lookup"><span data-stu-id="3a4ba-105">Get the [Focused Inbox](../resources/manage-focused-inbox.md) overrides that a user has set up to always classify messages from certain senders in specific ways.</span></span>

<span data-ttu-id="3a4ba-106">Cada substituição corresponde a um endereço SMTP de um remetente.</span><span class="sxs-lookup"><span data-stu-id="3a4ba-106">Each override corresponds to an SMTP address of a sender.</span></span> <span data-ttu-id="3a4ba-107">Inicialmente, um usuário não tem quaisquer substituições.</span><span class="sxs-lookup"><span data-stu-id="3a4ba-107">Initially, a user does not have any overrides.</span></span>
## <a name="permissions"></a><span data-ttu-id="3a4ba-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="3a4ba-108">Permissions</span></span>
<span data-ttu-id="3a4ba-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a4ba-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a4ba-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3a4ba-111">Permission type</span></span>      | <span data-ttu-id="3a4ba-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3a4ba-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3a4ba-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3a4ba-113">Delegated (work or school account)</span></span> | <span data-ttu-id="3a4ba-114">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="3a4ba-114">Mail.Read</span></span>    |
|<span data-ttu-id="3a4ba-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3a4ba-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3a4ba-116">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="3a4ba-116">Mail.Read</span></span>    |
|<span data-ttu-id="3a4ba-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3a4ba-117">Application</span></span> | <span data-ttu-id="3a4ba-118">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="3a4ba-118">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="3a4ba-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3a4ba-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/inferenceClassification/overrides
GET /users/{id}/inferenceClassification/overrides
```

## <a name="request-headers"></a><span data-ttu-id="3a4ba-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3a4ba-120">Request headers</span></span>
| <span data-ttu-id="3a4ba-121">Nome</span><span class="sxs-lookup"><span data-stu-id="3a4ba-121">Name</span></span>       | <span data-ttu-id="3a4ba-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="3a4ba-122">Type</span></span> | <span data-ttu-id="3a4ba-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="3a4ba-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="3a4ba-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="3a4ba-124">Authorization</span></span>  | <span data-ttu-id="3a4ba-125">string</span><span class="sxs-lookup"><span data-stu-id="3a4ba-125">string</span></span>  | <span data-ttu-id="3a4ba-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3a4ba-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3a4ba-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3a4ba-128">Request body</span></span>
<span data-ttu-id="3a4ba-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3a4ba-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3a4ba-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="3a4ba-130">Response</span></span>

<span data-ttu-id="3a4ba-131">Se bem sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3a4ba-131">If successful, this method returns a `200 OK` response code and a collection of [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3a4ba-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3a4ba-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3a4ba-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3a4ba-133">Request</span></span>
<span data-ttu-id="3a4ba-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3a4ba-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3a4ba-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="3a4ba-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_overrides"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/inferenceClassification/overrides
```
# <a name="c"></a>[<span data-ttu-id="3a4ba-136">C#</span><span class="sxs-lookup"><span data-stu-id="3a4ba-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-overrides-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3a4ba-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3a4ba-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-overrides-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3a4ba-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3a4ba-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-overrides-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="3a4ba-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="3a4ba-139">Response</span></span>
<span data-ttu-id="3a4ba-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3a4ba-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
