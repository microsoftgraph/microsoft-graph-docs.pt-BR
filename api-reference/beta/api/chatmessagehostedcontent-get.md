---
title: Obter chatMessageHostedContent
description: Recupere as propriedades e os relacionamentos do objeto chatMessageHostedContent.
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: d62ffb6fdf88649971992fc42e25ce16be6ae7ab
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42438292"
---
# <a name="get-chatmessagehostedcontent"></a><span data-ttu-id="cef92-103">Obter chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="cef92-103">Get chatMessageHostedContent</span></span>

<span data-ttu-id="cef92-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="cef92-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cef92-105">Recupere as propriedades e os relacionamentos do objeto [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) .</span><span class="sxs-lookup"><span data-stu-id="cef92-105">Retrieve the properties and relationships of [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="cef92-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="cef92-106">Permissions</span></span>

<span data-ttu-id="cef92-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cef92-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cef92-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cef92-109">Permission type</span></span>                        | <span data-ttu-id="cef92-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cef92-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="cef92-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cef92-111">Delegated (work or school account)</span></span>|<span data-ttu-id="cef92-112">Para o recurso de **usuário** ou **chat** :</span><span class="sxs-lookup"><span data-stu-id="cef92-112">For **user** or **chat** resource:</span></span><br/><span data-ttu-id="cef92-113">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cef92-113">Chat.Read, Chat.ReadWrite</span></span><br/><br/><span data-ttu-id="cef92-114">Para o recurso de **canal**:</span><span class="sxs-lookup"><span data-stu-id="cef92-114">For **channel** resource:</span></span><br/><span data-ttu-id="cef92-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cef92-115">Group.Read.All, Group.ReadWrite.All</span></span>|
|<span data-ttu-id="cef92-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cef92-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cef92-117">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="cef92-117">Not supported</span></span>|
|<span data-ttu-id="cef92-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cef92-118">Application</span></span>| <span data-ttu-id="cef92-119">Para o recurso de **usuário** ou **chat** :</span><span class="sxs-lookup"><span data-stu-id="cef92-119">For **user** or **chat** resource:</span></span><br/><span data-ttu-id="cef92-120">Chat.Read.All, Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cef92-120">Chat.Read.All, Chat.ReadWrite.All</span></span><br/><br/><span data-ttu-id="cef92-121">Para o recurso de **canal**:</span><span class="sxs-lookup"><span data-stu-id="cef92-121">For **channel** resource:</span></span><br/><span data-ttu-id="cef92-122">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cef92-122">Group.Read.All, Group.ReadWrite.All</span></span> |

> [!NOTE]
> <span data-ttu-id="cef92-123">É necessário solicitar acesso antes de chamar essa API com permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="cef92-123">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="cef92-124">Para obter detalhes, confira [APIs protegidas no Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="cef92-124">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="cef92-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cef92-125">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /chats/{id}/messages/{id}/hostedContents/{id}
GET /users/{id}/chats/{id}/messages/{id}/hostedContents/{id}
GET /teams/{id}/channels/{id}/messages/{id}/hostedContents/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cef92-126">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="cef92-126">Optional query parameters</span></span>

<span data-ttu-id="cef92-127">Esta operação não é compatível com os [parâmetros de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="cef92-127">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cef92-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cef92-128">Request headers</span></span>

| <span data-ttu-id="cef92-129">Nome</span><span class="sxs-lookup"><span data-stu-id="cef92-129">Name</span></span>      |<span data-ttu-id="cef92-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="cef92-130">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="cef92-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="cef92-131">Authorization</span></span> | <span data-ttu-id="cef92-132">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="cef92-132">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="cef92-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cef92-133">Request body</span></span>

<span data-ttu-id="cef92-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cef92-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cef92-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="cef92-135">Response</span></span>

<span data-ttu-id="cef92-136">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cef92-136">If successful, this method returns a `200 OK` response code and the requested [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cef92-137">Exemplos</span><span class="sxs-lookup"><span data-stu-id="cef92-137">Examples</span></span>

### <a name="example-1-get-hosted-content"></a><span data-ttu-id="cef92-138">Exemplo 1: obter conteúdo hospedado</span><span class="sxs-lookup"><span data-stu-id="cef92-138">Example 1: Get hosted content</span></span>

#### <a name="request"></a><span data-ttu-id="cef92-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cef92-139">Request</span></span>

<span data-ttu-id="cef92-140">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="cef92-140">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cef92-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="cef92-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chatmessagehostedcontent"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/chats/{id}/messages/{id}/hostedContents/{id}
```
# <a name="c"></a>[<span data-ttu-id="cef92-142">C#</span><span class="sxs-lookup"><span data-stu-id="cef92-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chatmessagehostedcontent-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cef92-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cef92-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chatmessagehostedcontent-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cef92-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cef92-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chatmessagehostedcontent-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="cef92-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="cef92-145">Response</span></span>

<span data-ttu-id="cef92-146">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="cef92-146">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="cef92-147">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="cef92-147">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="cef92-148">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cef92-148">All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-hosted-content-bytes-for-an-image"></a><span data-ttu-id="cef92-149">Exemplo 2: obter bytes de conteúdo hospedados para uma imagem</span><span class="sxs-lookup"><span data-stu-id="cef92-149">Example 2: Get hosted content bytes for an image</span></span>

#### <a name="request"></a><span data-ttu-id="cef92-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cef92-150">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="cef92-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="cef92-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chatmessagehostedcontent"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/chats/{id}/messages/{id}/hostedContents/{id}/$value
```
# <a name="c"></a>[<span data-ttu-id="cef92-152">C#</span><span class="sxs-lookup"><span data-stu-id="cef92-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chatmessagehostedcontent-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cef92-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cef92-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chatmessagehostedcontent-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cef92-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cef92-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chatmessagehostedcontent-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="cef92-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="cef92-155">Response</span></span>

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
