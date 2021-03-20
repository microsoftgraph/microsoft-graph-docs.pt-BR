---
title: Obter chatMessageHostedContent
description: Recupere as propriedades e as relações do objeto chatMessageHostedContent.
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 56c96c812c1c5f8e8a6d471224bf8faef2733045
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50947735"
---
# <a name="get-chatmessagehostedcontent"></a><span data-ttu-id="d969b-103">Obter chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="d969b-103">Get chatMessageHostedContent</span></span>

<span data-ttu-id="d969b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d969b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d969b-105">Recupere as propriedades e as relações do [objeto chatMessageHostedContent.](../resources/chatmessagehostedcontent.md)</span><span class="sxs-lookup"><span data-stu-id="d969b-105">Retrieve the properties and relationships of [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d969b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d969b-106">Permissions</span></span>

<span data-ttu-id="d969b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d969b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d969b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d969b-109">Permission type</span></span>                        | <span data-ttu-id="d969b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d969b-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="d969b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d969b-111">Delegated (work or school account)</span></span>| <span data-ttu-id="d969b-112">Para **o recurso** de usuário ou **chat:** Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d969b-112">For **user** or **chat** resource: Chat.Read, Chat.ReadWrite</span></span><br/><br/><span data-ttu-id="d969b-113">Para **recurso de** canal: ChannelMessage.Read.All, Group.Read.All, Group.Read.WriteAll</span><span class="sxs-lookup"><span data-stu-id="d969b-113">For **channel** resource: ChannelMessage.Read.All, Group.Read.All, Group.Read.WriteAll</span></span> |
|<span data-ttu-id="d969b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d969b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d969b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d969b-115">Not supported.</span></span>|
|<span data-ttu-id="d969b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d969b-116">Application</span></span>| <span data-ttu-id="d969b-117">Para **o recurso** de usuário ou **chat:** Chat.Read.All, Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d969b-117">For **user** or **chat** resource: Chat.Read.All, Chat.ReadWrite.All</span></span><br/><br/><span data-ttu-id="d969b-118">Para **recurso de** canal: ChannelMessage.Read.Group\*, ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d969b-118">For **channel** resource: ChannelMessage.Read.Group\*, ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> |

> <span data-ttu-id="d969b-119">**Observação**: Permissões marcadas com \* usam [consentimento específico de recurso]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="d969b-119">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> [!NOTE]
> <span data-ttu-id="d969b-120">É necessário solicitar acesso antes de chamar essa API com permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d969b-120">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="d969b-121">Para obter detalhes, confira [APIs protegidas no Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="d969b-121">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="d969b-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d969b-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /chats/{id}/messages/{id}/hostedContents/{id}
GET /users/{id}/chats/{id}/messages/{id}/hostedContents/{id}
GET /teams/{id}/channels/{id}/messages/{id}/hostedContents/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d969b-123">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d969b-123">Optional query parameters</span></span>

<span data-ttu-id="d969b-124">Esta operação não é compatível com os [parâmetros de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d969b-124">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d969b-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d969b-125">Request headers</span></span>

| <span data-ttu-id="d969b-126">Nome</span><span class="sxs-lookup"><span data-stu-id="d969b-126">Name</span></span>      |<span data-ttu-id="d969b-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="d969b-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d969b-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="d969b-128">Authorization</span></span> | <span data-ttu-id="d969b-129">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="d969b-129">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="d969b-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d969b-130">Request body</span></span>

<span data-ttu-id="d969b-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d969b-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d969b-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="d969b-132">Response</span></span>

<span data-ttu-id="d969b-133">Se tiver êxito, este método retornará um código de resposta e `200 OK` o [objeto chatMessageHostedContent](../resources/chatmessagehostedcontent.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d969b-133">If successful, this method returns a `200 OK` response code and the requested [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d969b-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d969b-134">Examples</span></span>

### <a name="example-1-get-hosted-content"></a><span data-ttu-id="d969b-135">Exemplo 1: Obter conteúdo hospedado</span><span class="sxs-lookup"><span data-stu-id="d969b-135">Example 1: Get hosted content</span></span>

#### <a name="request"></a><span data-ttu-id="d969b-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d969b-136">Request</span></span>

<span data-ttu-id="d969b-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d969b-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d969b-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="d969b-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chatmessagehostedcontent_1"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/chats/{id}/messages/{id}/hostedContents/{id}
```
# <a name="c"></a>[<span data-ttu-id="d969b-139">C#</span><span class="sxs-lookup"><span data-stu-id="d969b-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chatmessagehostedcontent-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d969b-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d969b-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chatmessagehostedcontent-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d969b-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d969b-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chatmessagehostedcontent-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d969b-142">Java</span><span class="sxs-lookup"><span data-stu-id="d969b-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-chatmessagehostedcontent-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="d969b-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="d969b-143">Response</span></span>

<span data-ttu-id="d969b-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d969b-144">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="d969b-145">O objeto de resposta mostrado aqui pode ser reduzido para a capacidade de leitura.</span><span class="sxs-lookup"><span data-stu-id="d969b-145">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d969b-146">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d969b-146">All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-hosted-content-bytes-for-an-image"></a><span data-ttu-id="d969b-147">Exemplo 2: Obter bytes de conteúdo hospedados para uma imagem</span><span class="sxs-lookup"><span data-stu-id="d969b-147">Example 2: Get hosted content bytes for an image</span></span>

#### <a name="request"></a><span data-ttu-id="d969b-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d969b-148">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="d969b-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="d969b-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chatmessagehostedcontent_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/chats/{id}/messages/{id}/hostedContents/{id}/$value
```
# <a name="c"></a>[<span data-ttu-id="d969b-150">C#</span><span class="sxs-lookup"><span data-stu-id="d969b-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chatmessagehostedcontent-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d969b-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d969b-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chatmessagehostedcontent-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d969b-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d969b-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chatmessagehostedcontent-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d969b-153">Java</span><span class="sxs-lookup"><span data-stu-id="d969b-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-chatmessagehostedcontent-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d969b-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="d969b-154">Response</span></span>

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


