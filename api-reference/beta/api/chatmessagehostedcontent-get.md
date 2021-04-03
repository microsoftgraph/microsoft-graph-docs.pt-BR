---
title: Obter chatMessageHostedContent
description: Recupere as propriedades e as relações do objeto chatMessageHostedContent.
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 23a62d1d25c442d4f305f3b68228712c97eff05b
ms.sourcegitcommit: 16ee16e7fddd662ca42dc5c9352cfb109e31ed1a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/03/2021
ms.locfileid: "51582659"
---
# <a name="get-chatmessagehostedcontent"></a><span data-ttu-id="aaca9-103">Obter chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="aaca9-103">Get chatMessageHostedContent</span></span>

<span data-ttu-id="aaca9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aaca9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aaca9-105">Recupere as propriedades e as relações do [objeto chatMessageHostedContent.](../resources/chatmessagehostedcontent.md)</span><span class="sxs-lookup"><span data-stu-id="aaca9-105">Retrieve the properties and relationships of [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="aaca9-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="aaca9-106">Permissions</span></span>

<span data-ttu-id="aaca9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aaca9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-for-channel"></a><span data-ttu-id="aaca9-109">Permissões para canal</span><span class="sxs-lookup"><span data-stu-id="aaca9-109">Permissions for channel</span></span>

| <span data-ttu-id="aaca9-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="aaca9-110">Permission type</span></span>                        | <span data-ttu-id="aaca9-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="aaca9-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="aaca9-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="aaca9-112">Delegated (work or school account)</span></span>| <span data-ttu-id="aaca9-113">ChannelMessage.Read.All, Group.Read.All, Group.Read.WriteAll</span><span class="sxs-lookup"><span data-stu-id="aaca9-113">ChannelMessage.Read.All, Group.Read.All, Group.Read.WriteAll</span></span> |
|<span data-ttu-id="aaca9-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="aaca9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aaca9-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aaca9-115">Not supported.</span></span>|
|<span data-ttu-id="aaca9-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="aaca9-116">Application</span></span>| <span data-ttu-id="aaca9-117">ChannelMessage.Read.Group, ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aaca9-117">ChannelMessage.Read.Group, ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> |

### <a name="permissions-for-chat"></a><span data-ttu-id="aaca9-118">Permissões para chat</span><span class="sxs-lookup"><span data-stu-id="aaca9-118">Permissions for chat</span></span>

| <span data-ttu-id="aaca9-119">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="aaca9-119">Permission type</span></span>                        | <span data-ttu-id="aaca9-120">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="aaca9-120">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="aaca9-121">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="aaca9-121">Delegated (work or school account)</span></span>| <span data-ttu-id="aaca9-122">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aaca9-122">Chat.Read, Chat.ReadWrite</span></span>|
|<span data-ttu-id="aaca9-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="aaca9-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aaca9-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aaca9-124">Not supported.</span></span>|
|<span data-ttu-id="aaca9-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="aaca9-125">Application</span></span>| <span data-ttu-id="aaca9-126">Chat.Read.All, Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aaca9-126">Chat.Read.All, Chat.ReadWrite.All</span></span>|

> <span data-ttu-id="aaca9-127">**Observação**: Permissões marcadas com \* usam [consentimento específico de recurso]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="aaca9-127">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> [!NOTE]
> <span data-ttu-id="aaca9-128">É necessário solicitar acesso antes de chamar essa API com permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="aaca9-128">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="aaca9-129">Para obter detalhes, confira [APIs protegidas no Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="aaca9-129">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="aaca9-130">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="aaca9-130">HTTP request</span></span>

<span data-ttu-id="aaca9-131">**Obter conteúdo hospedado em uma mensagem de canal**</span><span class="sxs-lookup"><span data-stu-id="aaca9-131">**Get hosted content in a channel message**</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{team-id}/channels/{channel-id}/messages/{message-id}/hostedContents/{hosted-content-id}
GET /teams/{team-id}/channels/{channel-id}/messages/{message-id}/replies/{reply-id}/hostedContents/{hosted-content-id}
```

<span data-ttu-id="aaca9-132">**Obter conteúdo hospedado em uma mensagem de chat**</span><span class="sxs-lookup"><span data-stu-id="aaca9-132">**Get hosted content in a chat message**</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /chats/{chat-id}/messages/{message-id}/hostedContents/{hosted-content-id}
GET /users/{user-id}/chats/{chat-id}/messages/{message-id}/hostedContents/{hosted-content-id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="aaca9-133">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="aaca9-133">Optional query parameters</span></span>

<span data-ttu-id="aaca9-134">Esta operação não é compatível com os [parâmetros de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="aaca9-134">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="aaca9-135">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="aaca9-135">Request headers</span></span>

| <span data-ttu-id="aaca9-136">Nome</span><span class="sxs-lookup"><span data-stu-id="aaca9-136">Name</span></span>      |<span data-ttu-id="aaca9-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="aaca9-137">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="aaca9-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="aaca9-138">Authorization</span></span> | <span data-ttu-id="aaca9-139">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="aaca9-139">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="aaca9-140">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="aaca9-140">Request body</span></span>

<span data-ttu-id="aaca9-141">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="aaca9-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aaca9-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="aaca9-142">Response</span></span>

<span data-ttu-id="aaca9-143">Se tiver êxito, este método retornará um código de resposta e `200 OK` o [objeto chatMessageHostedContent](../resources/chatmessagehostedcontent.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="aaca9-143">If successful, this method returns a `200 OK` response code and the requested [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="aaca9-144">Exemplos</span><span class="sxs-lookup"><span data-stu-id="aaca9-144">Examples</span></span>

### <a name="example-1-get-hosted-content-for-message-in-a-chat"></a><span data-ttu-id="aaca9-145">Exemplo 1: Obter conteúdo hospedado para mensagem em um chat</span><span class="sxs-lookup"><span data-stu-id="aaca9-145">Example 1: Get hosted content for message in a chat</span></span>

#### <a name="request"></a><span data-ttu-id="aaca9-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aaca9-146">Request</span></span>

<span data-ttu-id="aaca9-147">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="aaca9-147">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_hostedcontentchatmessage_1"
}-->
```http
GET https://graph.microsoft.com/beta/chats/19:2da4c29f6d7041eca70b638b43d45437@thread.v2/messages/1615971548136/hostedContents/aWQ9eF8wLXd1cy1kOS1lNTRmNjM1NWYxYmJkNGQ3ZTNmNGJhZmU4NTI5MTBmNix0eXBlPTEsdXJsPWh0dHBzOi8vdXMtYXBpLmFzbS5za3lwZS5jb20vdjEvb2JqZWN0cy8wLXd1cy1kOS1lNTRmNjM1NWYxYmJkNGQ3ZTNmNGJhZmU4NTI5MTBmNi92aWV3cy9pbWdv
```
#### <a name="response"></a><span data-ttu-id="aaca9-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="aaca9-148">Response</span></span>

<span data-ttu-id="aaca9-149">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="aaca9-149">The following is an example of the response.</span></span>

> <span data-ttu-id="aaca9-150">**Observação:** `contentBytes` e `contentType` são sempre definidos como nulos.</span><span class="sxs-lookup"><span data-stu-id="aaca9-150">**Note:** `contentBytes` and `contentType` are always set to null.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessageHostedContent"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#chats('19%3A2da4c29f6d7041eca70b638b43d45437%40thread.v2')/messages('1615971548136')/hostedContents/$entity",
    "id": "aWQ9eF8wLXd1cy1kOS1lNTRmNjM1NWYxYmJkNGQ3ZTNmNGJhZmU4NTI5MTBmNix0eXBlPTEsdXJsPWh0dHBzOi8vdXMtYXBpLmFzbS5za3lwZS5jb20vdjEvb2JqZWN0cy8wLXd1cy1kOS1lNTRmNjM1NWYxYmJkNGQ3ZTNmNGJhZmU4NTI5MTBmNi92aWV3cy9pbWdv",
    "contentBytes": null,
    "contentType": null
}
```

### <a name="example-2-get-hosted-content-bytes-for-an-image"></a><span data-ttu-id="aaca9-151">Exemplo 2: Obter bytes de conteúdo hospedados para uma imagem</span><span class="sxs-lookup"><span data-stu-id="aaca9-151">Example 2: Get hosted content bytes for an image</span></span>

#### <a name="request"></a><span data-ttu-id="aaca9-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aaca9-152">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_hostedcontentchatmessage_2"
}-->
```http
GET https://graph.microsoft.com/beta/chats/19:2da4c29f6d7041eca70b638b43d45437@thread.v2/messages/1615971548136/hostedContents/aWQ9eF8wLXd1cy1kOS1lNTRmNjM1NWYxYmJkNGQ3ZTNmNGJhZmU4NTI5MTBmNix0eXBlPTEsdXJsPWh0dHBzOi8vdXMtYXBpLmFzbS5za3lwZS5jb20vdjEvb2JqZWN0cy8wLXd1cy1kOS1lNTRmNjM1NWYxYmJkNGQ3ZTNmNGJhZmU4NTI5MTBmNi92aWV3cy9pbWdv/$value
```

#### <a name="response"></a><span data-ttu-id="aaca9-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="aaca9-153">Response</span></span>

<span data-ttu-id="aaca9-154">A resposta contém bytes para o conteúdo hospedado no corpo.</span><span class="sxs-lookup"><span data-stu-id="aaca9-154">Response contains bytes for the hosted content in the body.</span></span> <span data-ttu-id="aaca9-155">`content-type` o header especifica o tipo de conteúdo hospedado.</span><span class="sxs-lookup"><span data-stu-id="aaca9-155">`content-type` header specifies the kind of hosted content.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessageHostedContent"
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


