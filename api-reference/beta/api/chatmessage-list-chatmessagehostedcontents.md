---
title: Listar chatMessageHostedContents
description: Recupere a lista de objetos chatMessageHostedContent de uma mensagem.
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 019778894e9af80bf5ede1108bfd82ab7082a22a
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2020
ms.locfileid: "44287091"
---
# <a name="list-hostedcontents"></a><span data-ttu-id="42a2e-103">Listar hostedContents</span><span class="sxs-lookup"><span data-stu-id="42a2e-103">List hostedContents</span></span>

<span data-ttu-id="42a2e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="42a2e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="42a2e-105">Recupere a lista de objetos [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) de uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="42a2e-105">Retrieve the list of [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) objects from a message.</span></span>

## <a name="permissions"></a><span data-ttu-id="42a2e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="42a2e-106">Permissions</span></span>

<span data-ttu-id="42a2e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="42a2e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="42a2e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="42a2e-109">Permission type</span></span>                        | <span data-ttu-id="42a2e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="42a2e-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="42a2e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="42a2e-111">Delegated (work or school account)</span></span>| <span data-ttu-id="42a2e-112">Para recurso de **usuário** ou **chat** : chat. Read, chat. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="42a2e-112">For **user** or **chat** resource: Chat.Read, Chat.ReadWrite</span></span><br/><br/><span data-ttu-id="42a2e-113">Para recurso de **canal** : ChannelMessage. Read. All, Group. Read. All, Group. Read. WriteAll</span><span class="sxs-lookup"><span data-stu-id="42a2e-113">For **channel** resource: ChannelMessage.Read.All, Group.Read.All, Group.Read.WriteAll</span></span> |
|<span data-ttu-id="42a2e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="42a2e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="42a2e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="42a2e-115">Not supported.</span></span>|
|<span data-ttu-id="42a2e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="42a2e-116">Application</span></span>| <span data-ttu-id="42a2e-117">Para o **usuário** ou recurso de **chat** : chat. Read. All, chat. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="42a2e-117">For **user** or **chat** resource: Chat.Read.All, Chat.ReadWrite.All</span></span><br/><br/><span data-ttu-id="42a2e-118">Para o recurso de **canal** : ChannelMessage. Read. Group ([RSC](https://aka.ms/teams-rsc)), ChannelMessage. Read. All, Group. Read. All, Group. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="42a2e-118">For **channel** resource: ChannelMessage.Read.Group  ([RSC](https://aka.ms/teams-rsc)), ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> |

> [!NOTE]
> <span data-ttu-id="42a2e-119">É necessário solicitar acesso antes de chamar essa API com permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="42a2e-119">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="42a2e-120">Para obter detalhes, confira [APIs protegidas no Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="42a2e-120">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="42a2e-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="42a2e-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /chats/{id}/messages/{id}/hostedContents
GET /users/{id}/chats/{id}/messages/{id}/hostedContents
GET /teams/{id}/channels/{id}/messages/{id}/hostedContents
```

## <a name="optional-query-parameters"></a><span data-ttu-id="42a2e-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="42a2e-122">Optional query parameters</span></span>

<span data-ttu-id="42a2e-123">Esta operação não é compatível com os [parâmetros de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="42a2e-123">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="42a2e-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="42a2e-124">Request headers</span></span>

| <span data-ttu-id="42a2e-125">Nome</span><span class="sxs-lookup"><span data-stu-id="42a2e-125">Name</span></span>      |<span data-ttu-id="42a2e-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="42a2e-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="42a2e-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="42a2e-127">Authorization</span></span> | <span data-ttu-id="42a2e-128">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="42a2e-128">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="42a2e-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="42a2e-129">Request body</span></span>

<span data-ttu-id="42a2e-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="42a2e-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="42a2e-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="42a2e-131">Response</span></span>

<span data-ttu-id="42a2e-132">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="42a2e-132">If successful, this method returns a `200 OK` response code and a collection of [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="42a2e-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="42a2e-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="42a2e-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="42a2e-134">Request</span></span>

<span data-ttu-id="42a2e-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="42a2e-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="42a2e-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="42a2e-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_hostedcontents"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/chats/{id}/messages/{id}/hostedContents
```
# <a name="c"></a>[<span data-ttu-id="42a2e-137">C#</span><span class="sxs-lookup"><span data-stu-id="42a2e-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-hostedcontents-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="42a2e-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="42a2e-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-hostedcontents-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="42a2e-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="42a2e-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-hostedcontents-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="42a2e-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="42a2e-140">Response</span></span>

<span data-ttu-id="42a2e-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="42a2e-141">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="42a2e-142">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="42a2e-142">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="42a2e-143">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="42a2e-143">All the properties will be returned from an actual call.</span></span>

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
