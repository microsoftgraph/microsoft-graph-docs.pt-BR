---
title: Listar chatMessageHostedContents
description: Recupere a lista de objetos chatMessageHostedContent de uma mensagem.
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 0be0b5668b4e583b855ae4e4e85fdb7bc4169705
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42438369"
---
# <a name="list-hostedcontents"></a><span data-ttu-id="ab191-103">Listar hostedContents</span><span class="sxs-lookup"><span data-stu-id="ab191-103">List hostedContents</span></span>

<span data-ttu-id="ab191-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ab191-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ab191-105">Recupere a lista de objetos [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) de uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="ab191-105">Retrieve the list of [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) objects from a message.</span></span>

## <a name="permissions"></a><span data-ttu-id="ab191-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ab191-106">Permissions</span></span>

<span data-ttu-id="ab191-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ab191-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ab191-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ab191-109">Permission type</span></span>                        | <span data-ttu-id="ab191-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ab191-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="ab191-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ab191-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ab191-112">Para o recurso de **usuário** ou **chat** :</span><span class="sxs-lookup"><span data-stu-id="ab191-112">For **user** or **chat** resource:</span></span><br/><span data-ttu-id="ab191-113">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ab191-113">Chat.Read, Chat.ReadWrite</span></span><br/><br/><span data-ttu-id="ab191-114">Para o recurso de **canal**:</span><span class="sxs-lookup"><span data-stu-id="ab191-114">For **channel** resource:</span></span><br/><span data-ttu-id="ab191-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab191-115">Group.Read.All, Group.ReadWrite.All</span></span>|
|<span data-ttu-id="ab191-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ab191-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ab191-117">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="ab191-117">Not supported</span></span>|
|<span data-ttu-id="ab191-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ab191-118">Application</span></span>| <span data-ttu-id="ab191-119">Para o recurso de **usuário** ou **chat** :</span><span class="sxs-lookup"><span data-stu-id="ab191-119">For **user** or **chat** resource:</span></span><br/><span data-ttu-id="ab191-120">Chat.Read.All, Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab191-120">Chat.Read.All, Chat.ReadWrite.All</span></span><br/><br/><span data-ttu-id="ab191-121">Para o recurso de **canal**:</span><span class="sxs-lookup"><span data-stu-id="ab191-121">For **channel** resource:</span></span><br/><span data-ttu-id="ab191-122">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab191-122">Group.Read.All, Group.ReadWrite.All</span></span> |

> [!NOTE]
> <span data-ttu-id="ab191-123">É necessário solicitar acesso antes de chamar essa API com permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ab191-123">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="ab191-124">Para obter detalhes, confira [APIs protegidas no Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="ab191-124">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="ab191-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ab191-125">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /chats/{id}/messages/{id}/hostedContents
GET /users/{id}/chats/{id}/messages/{id}/hostedContents
GET /teams/{id}/channels/{id}/messages/{id}/hostedContents
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ab191-126">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ab191-126">Optional query parameters</span></span>

<span data-ttu-id="ab191-127">Esta operação não é compatível com os [parâmetros de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ab191-127">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ab191-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ab191-128">Request headers</span></span>

| <span data-ttu-id="ab191-129">Nome</span><span class="sxs-lookup"><span data-stu-id="ab191-129">Name</span></span>      |<span data-ttu-id="ab191-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="ab191-130">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ab191-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="ab191-131">Authorization</span></span> | <span data-ttu-id="ab191-132">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="ab191-132">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="ab191-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ab191-133">Request body</span></span>

<span data-ttu-id="ab191-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ab191-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ab191-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="ab191-135">Response</span></span>

<span data-ttu-id="ab191-136">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ab191-136">If successful, this method returns a `200 OK` response code and a collection of [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ab191-137">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ab191-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ab191-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ab191-138">Request</span></span>

<span data-ttu-id="ab191-139">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ab191-139">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ab191-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="ab191-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_hostedcontents"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/chats/{id}/messages/{id}/hostedContents
```
# <a name="c"></a>[<span data-ttu-id="ab191-141">C#</span><span class="sxs-lookup"><span data-stu-id="ab191-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-hostedcontents-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ab191-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ab191-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-hostedcontents-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ab191-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ab191-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-hostedcontents-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ab191-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="ab191-144">Response</span></span>

<span data-ttu-id="ab191-145">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ab191-145">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="ab191-146">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ab191-146">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="ab191-147">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ab191-147">All the properties will be returned from an actual call.</span></span>

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
