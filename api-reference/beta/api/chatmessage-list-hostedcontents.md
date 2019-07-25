---
title: Listar hostedContents
description: Recupere uma lista de objetos chatMessageHostedContent.
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: b69379d77b2850e897ecce652f7ee2533f510a17
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35863555"
---
# <a name="list-hostedcontents"></a><span data-ttu-id="b7cc3-103">Listar hostedContents</span><span class="sxs-lookup"><span data-stu-id="b7cc3-103">List hostedContents</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b7cc3-104">Recupere uma lista de objetos [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) .</span><span class="sxs-lookup"><span data-stu-id="b7cc3-104">Retrieve a list of [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="b7cc3-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="b7cc3-105">Permissions</span></span>

<span data-ttu-id="b7cc3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b7cc3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b7cc3-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b7cc3-108">Permission type</span></span>                        | <span data-ttu-id="b7cc3-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b7cc3-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b7cc3-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b7cc3-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="b7cc3-111">Chat. Read, chat. ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="b7cc3-111">Chat.Read, Chat.ReadWrite.</span></span> |
| <span data-ttu-id="b7cc3-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b7cc3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b7cc3-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b7cc3-113">Not supported.</span></span> |
| <span data-ttu-id="b7cc3-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b7cc3-114">Application</span></span>                            | <span data-ttu-id="b7cc3-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b7cc3-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b7cc3-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b7cc3-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /chats/{id}/messages/{id}/hostedContents
GET /users/{id}/chats/{id}/messages/{id}/hostedContents
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b7cc3-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b7cc3-117">Optional query parameters</span></span>

<span data-ttu-id="b7cc3-118">Esta operação não oferece suporte aos [parâmetros de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b7cc3-118">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b7cc3-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b7cc3-119">Request headers</span></span>

| <span data-ttu-id="b7cc3-120">Nome</span><span class="sxs-lookup"><span data-stu-id="b7cc3-120">Name</span></span>      |<span data-ttu-id="b7cc3-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="b7cc3-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b7cc3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b7cc3-122">Authorization</span></span> | <span data-ttu-id="b7cc3-123">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="b7cc3-123">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="b7cc3-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b7cc3-124">Request body</span></span>

<span data-ttu-id="b7cc3-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b7cc3-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b7cc3-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="b7cc3-126">Response</span></span>

<span data-ttu-id="b7cc3-127">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b7cc3-127">If successful, this method returns a `200 OK` response code and a collection of [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b7cc3-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b7cc3-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b7cc3-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b7cc3-129">Request</span></span>

<span data-ttu-id="b7cc3-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b7cc3-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b7cc3-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="b7cc3-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_hostedcontents"
}-->

```http
GET https://graph.microsoft.com/beta/chats/{id}/messages/{id}/hostedContents
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b7cc3-132">C#</span><span class="sxs-lookup"><span data-stu-id="b7cc3-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-hostedcontents-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b7cc3-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="b7cc3-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-hostedcontents-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b7cc3-134">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="b7cc3-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-hostedcontents-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b7cc3-135">Java</span><span class="sxs-lookup"><span data-stu-id="b7cc3-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-hostedcontents-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b7cc3-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="b7cc3-136">Response</span></span>

<span data-ttu-id="b7cc3-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b7cc3-137">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="b7cc3-138">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b7cc3-138">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="b7cc3-139">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b7cc3-139">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessageHostedContent",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List hostedContents",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
