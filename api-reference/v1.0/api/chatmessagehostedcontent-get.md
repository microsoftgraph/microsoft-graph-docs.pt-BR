---
title: Obter chatMessageHostedContent
description: Recupere as propriedades e as relações do objeto chatMessageHostedContent.
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 2d74a55c5e0ddfe00a92912df75ed5fb0b166660
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787657"
---
# <a name="get-chatmessagehostedcontent"></a><span data-ttu-id="a4c38-103">Obter chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="a4c38-103">Get chatMessageHostedContent</span></span>

<span data-ttu-id="a4c38-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a4c38-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a4c38-105">Recupere as propriedades e as relações do [objeto chatMessageHostedContent.](../resources/chatmessagehostedcontent.md)</span><span class="sxs-lookup"><span data-stu-id="a4c38-105">Retrieve the properties and relationships of [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a4c38-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a4c38-106">Permissions</span></span>

<span data-ttu-id="a4c38-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a4c38-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-for-channel"></a><span data-ttu-id="a4c38-109">Permissões para o canal</span><span class="sxs-lookup"><span data-stu-id="a4c38-109">Permissions for channel</span></span>

| <span data-ttu-id="a4c38-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a4c38-110">Permission type</span></span>                        | <span data-ttu-id="a4c38-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a4c38-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="a4c38-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a4c38-112">Delegated (work or school account)</span></span>| <span data-ttu-id="a4c38-113">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="a4c38-113">ChannelMessage.Read.All</span></span> |
|<span data-ttu-id="a4c38-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a4c38-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a4c38-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a4c38-115">Not supported.</span></span>|
|<span data-ttu-id="a4c38-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a4c38-116">Application</span></span>| <span data-ttu-id="a4c38-117">ChannelMessage.Read.Group, ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="a4c38-117">ChannelMessage.Read.Group, ChannelMessage.Read.All</span></span> |

### <a name="permissions-for-chat"></a><span data-ttu-id="a4c38-118">Permissões para o chat</span><span class="sxs-lookup"><span data-stu-id="a4c38-118">Permissions for chat</span></span>

| <span data-ttu-id="a4c38-119">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a4c38-119">Permission type</span></span>                        | <span data-ttu-id="a4c38-120">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a4c38-120">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="a4c38-121">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a4c38-121">Delegated (work or school account)</span></span>| <span data-ttu-id="a4c38-122">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a4c38-122">Chat.Read, Chat.ReadWrite</span></span>|
|<span data-ttu-id="a4c38-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a4c38-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a4c38-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a4c38-124">Not supported.</span></span>|
|<span data-ttu-id="a4c38-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a4c38-125">Application</span></span>| <span data-ttu-id="a4c38-126">Chat.Read.All, Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4c38-126">Chat.Read.All, Chat.ReadWrite.All</span></span>|

> <span data-ttu-id="a4c38-127">**Observação**: Permissões marcadas com \* usam [consentimento específico de recurso]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="a4c38-127">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> [!NOTE]
> <span data-ttu-id="a4c38-128">É necessário solicitar acesso antes de chamar essa API com permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a4c38-128">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="a4c38-129">Para obter detalhes, confira [APIs protegidas no Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="a4c38-129">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="a4c38-130">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a4c38-130">HTTP request</span></span>

<span data-ttu-id="a4c38-131">**Obter conteúdo hospedado em uma mensagem de canal**</span><span class="sxs-lookup"><span data-stu-id="a4c38-131">**Get hosted content in a channel message**</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{team-id}/channels/{channel-id}/messages/{message-id}/hostedContents/{hosted-content-id}
GET /teams/{team-id}/channels/{channel-id}/messages/{message-id}/replies/{reply-id}/hostedContents/{hosted-content-id}
```

<span data-ttu-id="a4c38-132">**Obter conteúdo hospedado em uma mensagem de chat**</span><span class="sxs-lookup"><span data-stu-id="a4c38-132">**Get hosted content in a chat message**</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /chats/{chat-id}/messages/{message-id}/hostedContents/{hosted-content-id}
GET /users/{user-id | user-principal-name}/chats/{chat-id}/messages/{message-id}/hostedContents/{hosted-content-id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a4c38-133">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a4c38-133">Optional query parameters</span></span>

<span data-ttu-id="a4c38-134">Esta operação não é compatível com os [parâmetros de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a4c38-134">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a4c38-135">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a4c38-135">Request headers</span></span>

| <span data-ttu-id="a4c38-136">Nome</span><span class="sxs-lookup"><span data-stu-id="a4c38-136">Name</span></span>      |<span data-ttu-id="a4c38-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="a4c38-137">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a4c38-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="a4c38-138">Authorization</span></span> | <span data-ttu-id="a4c38-139">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="a4c38-139">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="a4c38-140">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a4c38-140">Request body</span></span>

<span data-ttu-id="a4c38-141">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a4c38-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a4c38-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="a4c38-142">Response</span></span>

<span data-ttu-id="a4c38-143">Se tiver êxito, este método retornará um código de resposta e `200 OK` o [objeto chatMessageHostedContent](../resources/chatmessagehostedcontent.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a4c38-143">If successful, this method returns a `200 OK` response code and the requested [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a4c38-144">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a4c38-144">Examples</span></span>

### <a name="example-1-get-hosted-content-for-message-in-a-chat"></a><span data-ttu-id="a4c38-145">Exemplo 1: Obter conteúdo hospedado para mensagem em um chat</span><span class="sxs-lookup"><span data-stu-id="a4c38-145">Example 1: Get hosted content for message in a chat</span></span>

#### <a name="request"></a><span data-ttu-id="a4c38-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a4c38-146">Request</span></span>

<span data-ttu-id="a4c38-147">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a4c38-147">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="a4c38-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="a4c38-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_hostedcontentchatmessage_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/chats/19:2da4c29f6d7041eca70b638b43d45437@thread.v2/messages/1615971548136/hostedContents/aWQ9eF8wLXd1cy1kOS1lNTRmNjM1NWYxYmJkNGQ3ZTNmNGJhZmU4NTI5MTBmNix0eXBlPTEsdXJsPWh0dHBzOi8vdXMtYXBpLmFzbS5za3lwZS5jb20vdjEvb2JqZWN0cy8wLXd1cy1kOS1lNTRmNjM1NWYxYmJkNGQ3ZTNmNGJhZmU4NTI5MTBmNi92aWV3cy9pbWdv
```
# <a name="c"></a>[<span data-ttu-id="a4c38-149">C#</span><span class="sxs-lookup"><span data-stu-id="a4c38-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-hostedcontentchatmessage-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a4c38-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a4c38-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-hostedcontentchatmessage-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a4c38-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a4c38-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-hostedcontentchatmessage-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a4c38-152">Java</span><span class="sxs-lookup"><span data-stu-id="a4c38-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-hostedcontentchatmessage-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="a4c38-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="a4c38-153">Response</span></span>

<span data-ttu-id="a4c38-154">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a4c38-154">The following is an example of the response.</span></span>

> <span data-ttu-id="a4c38-155">**Observação:** `contentBytes` e `contentType` são sempre definidos como nulos.</span><span class="sxs-lookup"><span data-stu-id="a4c38-155">**Note:** `contentBytes` and `contentType` are always set to null.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessageHostedContent"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#chats('19%3A2da4c29f6d7041eca70b638b43d45437%40thread.v2')/messages('1615971548136')/hostedContents/$entity",
    "id": "aWQ9eF8wLXd1cy1kOS1lNTRmNjM1NWYxYmJkNGQ3ZTNmNGJhZmU4NTI5MTBmNix0eXBlPTEsdXJsPWh0dHBzOi8vdXMtYXBpLmFzbS5za3lwZS5jb20vdjEvb2JqZWN0cy8wLXd1cy1kOS1lNTRmNjM1NWYxYmJkNGQ3ZTNmNGJhZmU4NTI5MTBmNi92aWV3cy9pbWdv",
    "contentBytes": null,
    "contentType": null
}
```

### <a name="example-2-get-hosted-content-bytes-for-an-image"></a><span data-ttu-id="a4c38-156">Exemplo 2: Obter bytes de conteúdo hospedados para uma imagem</span><span class="sxs-lookup"><span data-stu-id="a4c38-156">Example 2: Get hosted content bytes for an image</span></span>

#### <a name="request"></a><span data-ttu-id="a4c38-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a4c38-157">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="a4c38-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="a4c38-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_hostedcontentchatmessage_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/chats/19:2da4c29f6d7041eca70b638b43d45437@thread.v2/messages/1615971548136/hostedContents/aWQ9eF8wLXd1cy1kOS1lNTRmNjM1NWYxYmJkNGQ3ZTNmNGJhZmU4NTI5MTBmNix0eXBlPTEsdXJsPWh0dHBzOi8vdXMtYXBpLmFzbS5za3lwZS5jb20vdjEvb2JqZWN0cy8wLXd1cy1kOS1lNTRmNjM1NWYxYmJkNGQ3ZTNmNGJhZmU4NTI5MTBmNi92aWV3cy9pbWdv/$value
```
# <a name="c"></a>[<span data-ttu-id="a4c38-159">C#</span><span class="sxs-lookup"><span data-stu-id="a4c38-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-hostedcontentchatmessage-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a4c38-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a4c38-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-hostedcontentchatmessage-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a4c38-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a4c38-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-hostedcontentchatmessage-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a4c38-162">Java</span><span class="sxs-lookup"><span data-stu-id="a4c38-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-hostedcontentchatmessage-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a4c38-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="a4c38-163">Response</span></span>

<span data-ttu-id="a4c38-164">A resposta contém bytes para o conteúdo hospedado no corpo.</span><span class="sxs-lookup"><span data-stu-id="a4c38-164">Response contains bytes for the hosted content in the body.</span></span> <span data-ttu-id="a4c38-165">`content-type` o header especifica o tipo de conteúdo hospedado.</span><span class="sxs-lookup"><span data-stu-id="a4c38-165">`content-type` header specifies the kind of hosted content.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 200 OK
content-type: image/png
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


