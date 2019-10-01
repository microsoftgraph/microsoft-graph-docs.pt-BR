---
title: Listar chatMessageHostedContents
description: Recupere a lista de objetos chatMessageHostedContent de uma mensagem.
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: a39071d71728b6e510734ab05109f7c94a8a0e7f
ms.sourcegitcommit: 2fb178ae78b5ecc47207d2b19d0c5a46e07e0960
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/01/2019
ms.locfileid: "37333379"
---
# <a name="list-hostedcontents"></a><span data-ttu-id="c22fb-103">Listar hostedContents</span><span class="sxs-lookup"><span data-stu-id="c22fb-103">List hostedContents</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c22fb-104">Recupere a lista de objetos [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) de uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="c22fb-104">Retrieve the list of [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) objects from a message.</span></span>

## <a name="permissions"></a><span data-ttu-id="c22fb-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="c22fb-105">Permissions</span></span>

<span data-ttu-id="c22fb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c22fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c22fb-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c22fb-108">Permission type</span></span>                        | <span data-ttu-id="c22fb-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c22fb-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="c22fb-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c22fb-110">Delegated (work or school account)</span></span>|<span data-ttu-id="c22fb-111">Para o **usuário** ou recurso de **chat** :</span><span class="sxs-lookup"><span data-stu-id="c22fb-111">For **user** or **chat** resource:</span></span><br/><span data-ttu-id="c22fb-112">Chat. Read, chat. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c22fb-112">Chat.Read, Chat.ReadWrite</span></span><br/><br/><span data-ttu-id="c22fb-113">Para o recurso de **canal** :</span><span class="sxs-lookup"><span data-stu-id="c22fb-113">For **channel** resource:</span></span><br/><span data-ttu-id="c22fb-114">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c22fb-114">Group.Read.All, Group.ReadWrite.All</span></span>|
|<span data-ttu-id="c22fb-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c22fb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c22fb-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="c22fb-116">Not supported</span></span>|
|<span data-ttu-id="c22fb-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c22fb-117">Application</span></span>| <span data-ttu-id="c22fb-118">Para o **usuário** ou recurso de **chat** :</span><span class="sxs-lookup"><span data-stu-id="c22fb-118">For **user** or **chat** resource:</span></span><br/><span data-ttu-id="c22fb-119">Chat. Read. All, chat. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="c22fb-119">Chat.Read.All, Chat.ReadWrite.All</span></span><br/><br/><span data-ttu-id="c22fb-120">Para o recurso de **canal** :</span><span class="sxs-lookup"><span data-stu-id="c22fb-120">For **channel** resource:</span></span><br/><span data-ttu-id="c22fb-121">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c22fb-121">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c22fb-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c22fb-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /chats/{id}/messages/{id}/hostedContents
GET /users/{id}/chats/{id}/messages/{id}/hostedContents
GET /teams/{id}/channels/{id}/messages/{id}/hostedContents
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c22fb-123">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c22fb-123">Optional query parameters</span></span>

<span data-ttu-id="c22fb-124">Esta operação não oferece suporte aos [parâmetros de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c22fb-124">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c22fb-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c22fb-125">Request headers</span></span>

| <span data-ttu-id="c22fb-126">Nome</span><span class="sxs-lookup"><span data-stu-id="c22fb-126">Name</span></span>      |<span data-ttu-id="c22fb-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="c22fb-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c22fb-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="c22fb-128">Authorization</span></span> | <span data-ttu-id="c22fb-129">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="c22fb-129">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="c22fb-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c22fb-130">Request body</span></span>

<span data-ttu-id="c22fb-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c22fb-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c22fb-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="c22fb-132">Response</span></span>

<span data-ttu-id="c22fb-133">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c22fb-133">If successful, this method returns a `200 OK` response code and a collection of [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c22fb-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c22fb-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c22fb-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c22fb-135">Request</span></span>

<span data-ttu-id="c22fb-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c22fb-136">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c22fb-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="c22fb-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_hostedcontents"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/chats/{id}/messages/{id}/hostedContents
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c22fb-138">C#</span><span class="sxs-lookup"><span data-stu-id="c22fb-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-hostedcontents-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c22fb-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c22fb-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-hostedcontents-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c22fb-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c22fb-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-hostedcontents-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c22fb-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="c22fb-141">Response</span></span>

<span data-ttu-id="c22fb-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c22fb-142">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="c22fb-143">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c22fb-143">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c22fb-144">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c22fb-144">All the properties will be returned from an actual call.</span></span>

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
