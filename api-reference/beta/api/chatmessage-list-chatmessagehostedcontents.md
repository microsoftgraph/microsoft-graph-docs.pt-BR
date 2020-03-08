---
title: Listar chatMessageHostedContents
description: Recupere a lista de objetos chatMessageHostedContent de uma mensagem.
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 50459ee2ec043773480e40d9d3bf3f011f5528d1
ms.sourcegitcommit: 435d80cfa71574c06d24780c591d4303a5cd9636
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2020
ms.locfileid: "42562693"
---
# <a name="list-hostedcontents"></a><span data-ttu-id="aa714-103">Listar hostedContents</span><span class="sxs-lookup"><span data-stu-id="aa714-103">List hostedContents</span></span>

<span data-ttu-id="aa714-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aa714-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aa714-105">Recupere a lista de objetos [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) de uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="aa714-105">Retrieve the list of [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) objects from a message.</span></span>

## <a name="permissions"></a><span data-ttu-id="aa714-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="aa714-106">Permissions</span></span>

<span data-ttu-id="aa714-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aa714-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="aa714-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="aa714-109">Permission type</span></span>                        | <span data-ttu-id="aa714-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="aa714-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="aa714-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="aa714-111">Delegated (work or school account)</span></span>|<span data-ttu-id="aa714-112">Para o recurso de **usuário** ou **chat** :</span><span class="sxs-lookup"><span data-stu-id="aa714-112">For **user** or **chat** resource:</span></span><br/><span data-ttu-id="aa714-113">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aa714-113">Chat.Read, Chat.ReadWrite</span></span><br/><br/><span data-ttu-id="aa714-114">Para o recurso de **canal**:</span><span class="sxs-lookup"><span data-stu-id="aa714-114">For **channel** resource:</span></span><br/><span data-ttu-id="aa714-115">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa714-115">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span>|
|<span data-ttu-id="aa714-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="aa714-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aa714-117">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="aa714-117">Not supported</span></span>|
|<span data-ttu-id="aa714-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="aa714-118">Application</span></span>| <span data-ttu-id="aa714-119">Para o recurso de **usuário** ou **chat** :</span><span class="sxs-lookup"><span data-stu-id="aa714-119">For **user** or **chat** resource:</span></span><br/><span data-ttu-id="aa714-120">Chat.Read.All, Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa714-120">Chat.Read.All, Chat.ReadWrite.All</span></span><br/><br/><span data-ttu-id="aa714-121">Para o recurso de **canal**:</span><span class="sxs-lookup"><span data-stu-id="aa714-121">For **channel** resource:</span></span><br/><span data-ttu-id="aa714-122">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa714-122">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> |

> [!NOTE]
> <span data-ttu-id="aa714-123">É necessário solicitar acesso antes de chamar essa API com permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="aa714-123">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="aa714-124">Para obter detalhes, confira [APIs protegidas no Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="aa714-124">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="aa714-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="aa714-125">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /chats/{id}/messages/{id}/hostedContents
GET /users/{id}/chats/{id}/messages/{id}/hostedContents
GET /teams/{id}/channels/{id}/messages/{id}/hostedContents
```

## <a name="optional-query-parameters"></a><span data-ttu-id="aa714-126">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="aa714-126">Optional query parameters</span></span>

<span data-ttu-id="aa714-127">Esta operação não é compatível com os [parâmetros de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="aa714-127">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="aa714-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="aa714-128">Request headers</span></span>

| <span data-ttu-id="aa714-129">Nome</span><span class="sxs-lookup"><span data-stu-id="aa714-129">Name</span></span>      |<span data-ttu-id="aa714-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="aa714-130">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="aa714-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="aa714-131">Authorization</span></span> | <span data-ttu-id="aa714-132">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="aa714-132">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="aa714-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="aa714-133">Request body</span></span>

<span data-ttu-id="aa714-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="aa714-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aa714-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="aa714-135">Response</span></span>

<span data-ttu-id="aa714-136">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="aa714-136">If successful, this method returns a `200 OK` response code and a collection of [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="aa714-137">Exemplos</span><span class="sxs-lookup"><span data-stu-id="aa714-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="aa714-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aa714-138">Request</span></span>

<span data-ttu-id="aa714-139">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="aa714-139">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="aa714-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="aa714-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_hostedcontents"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/chats/{id}/messages/{id}/hostedContents
```
# <a name="c"></a>[<span data-ttu-id="aa714-141">C#</span><span class="sxs-lookup"><span data-stu-id="aa714-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-hostedcontents-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="aa714-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="aa714-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-hostedcontents-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="aa714-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="aa714-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-hostedcontents-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="aa714-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="aa714-144">Response</span></span>

<span data-ttu-id="aa714-145">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="aa714-145">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="aa714-146">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="aa714-146">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="aa714-147">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="aa714-147">All the properties will be returned from an actual call.</span></span>

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
