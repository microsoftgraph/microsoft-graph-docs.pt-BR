---
title: Obter chatMessageHostedContent
description: Recupere as propriedades e os relacionamentos do objeto chatMessageHostedContent.
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 81017fbf7dcf3aa2191131e8547cadc0175e60b5
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2020
ms.locfileid: "44287021"
---
# <a name="get-chatmessagehostedcontent"></a><span data-ttu-id="6efff-103">Obter chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="6efff-103">Get chatMessageHostedContent</span></span>

<span data-ttu-id="6efff-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6efff-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6efff-105">Recupere as propriedades e os relacionamentos do objeto [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) .</span><span class="sxs-lookup"><span data-stu-id="6efff-105">Retrieve the properties and relationships of [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6efff-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6efff-106">Permissions</span></span>

<span data-ttu-id="6efff-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6efff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6efff-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6efff-109">Permission type</span></span>                        | <span data-ttu-id="6efff-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6efff-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="6efff-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6efff-111">Delegated (work or school account)</span></span>| <span data-ttu-id="6efff-112">Para recurso de **usuário** ou **chat** : chat. Read, chat. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6efff-112">For **user** or **chat** resource: Chat.Read, Chat.ReadWrite</span></span><br/><br/><span data-ttu-id="6efff-113">Para recurso de **canal** : ChannelMessage. Read. All, Group. Read. All, Group. Read. WriteAll</span><span class="sxs-lookup"><span data-stu-id="6efff-113">For **channel** resource: ChannelMessage.Read.All, Group.Read.All, Group.Read.WriteAll</span></span> |
|<span data-ttu-id="6efff-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6efff-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6efff-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6efff-115">Not supported.</span></span>|
|<span data-ttu-id="6efff-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6efff-116">Application</span></span>| <span data-ttu-id="6efff-117">Para o **usuário** ou recurso de **chat** : chat. Read. All, chat. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="6efff-117">For **user** or **chat** resource: Chat.Read.All, Chat.ReadWrite.All</span></span><br/><br/><span data-ttu-id="6efff-118">Para o recurso de **canal** : ChannelMessage. Read. Group ([RSC](https://aka.ms/teams-rsc)), ChannelMessage. Read. All, Group. Read. All, Group. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="6efff-118">For **channel** resource: ChannelMessage.Read.Group  ([RSC](https://aka.ms/teams-rsc)), ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> |

> [!NOTE]
> <span data-ttu-id="6efff-119">É necessário solicitar acesso antes de chamar essa API com permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6efff-119">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="6efff-120">Para obter detalhes, confira [APIs protegidas no Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="6efff-120">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="6efff-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6efff-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /chats/{id}/messages/{id}/hostedContents/{id}
GET /users/{id}/chats/{id}/messages/{id}/hostedContents/{id}
GET /teams/{id}/channels/{id}/messages/{id}/hostedContents/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6efff-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6efff-122">Optional query parameters</span></span>

<span data-ttu-id="6efff-123">Esta operação não é compatível com os [parâmetros de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6efff-123">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6efff-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6efff-124">Request headers</span></span>

| <span data-ttu-id="6efff-125">Nome</span><span class="sxs-lookup"><span data-stu-id="6efff-125">Name</span></span>      |<span data-ttu-id="6efff-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="6efff-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6efff-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="6efff-127">Authorization</span></span> | <span data-ttu-id="6efff-128">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="6efff-128">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="6efff-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6efff-129">Request body</span></span>

<span data-ttu-id="6efff-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6efff-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6efff-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="6efff-131">Response</span></span>

<span data-ttu-id="6efff-132">Se tiver êxito, este método retornará um `200 OK` código de resposta e o objeto [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6efff-132">If successful, this method returns a `200 OK` response code and the requested [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6efff-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="6efff-133">Examples</span></span>

### <a name="example-1-get-hosted-content"></a><span data-ttu-id="6efff-134">Exemplo 1: obter conteúdo hospedado</span><span class="sxs-lookup"><span data-stu-id="6efff-134">Example 1: Get hosted content</span></span>

#### <a name="request"></a><span data-ttu-id="6efff-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6efff-135">Request</span></span>

<span data-ttu-id="6efff-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6efff-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6efff-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="6efff-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chatmessagehostedcontent"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/chats/{id}/messages/{id}/hostedContents/{id}
```
# <a name="c"></a>[<span data-ttu-id="6efff-138">C#</span><span class="sxs-lookup"><span data-stu-id="6efff-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chatmessagehostedcontent-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6efff-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6efff-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chatmessagehostedcontent-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6efff-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6efff-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chatmessagehostedcontent-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="6efff-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="6efff-141">Response</span></span>

<span data-ttu-id="6efff-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6efff-142">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="6efff-143">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="6efff-143">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="6efff-144">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6efff-144">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessageHostedContent"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "id-value"
}
```

### <a name="example-2-get-hosted-content-bytes-for-an-image"></a><span data-ttu-id="6efff-145">Exemplo 2: obter bytes de conteúdo hospedados para uma imagem</span><span class="sxs-lookup"><span data-stu-id="6efff-145">Example 2: Get hosted content bytes for an image</span></span>

#### <a name="request"></a><span data-ttu-id="6efff-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6efff-146">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="6efff-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="6efff-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chatmessagehostedcontent"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/chats/{id}/messages/{id}/hostedContents/{id}/$value
```
# <a name="c"></a>[<span data-ttu-id="6efff-148">C#</span><span class="sxs-lookup"><span data-stu-id="6efff-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chatmessagehostedcontent-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6efff-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6efff-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chatmessagehostedcontent-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6efff-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6efff-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chatmessagehostedcontent-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6efff-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="6efff-151">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessageHostedContent"
} -->

```http
HTTP/1.1 200 OK
Content-type: image/jpeg
Content-length: 201
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get chatMessageHostedContent",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
