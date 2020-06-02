---
title: Obter chatMessageHostedContent
description: Recupere as propriedades e os relacionamentos do objeto chatMessageHostedContent.
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: b9cbbfe106af827d34f7bdbcc50af03c59ec5aeb
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44491263"
---
# <a name="get-chatmessagehostedcontent"></a><span data-ttu-id="cbda0-103">Obter chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="cbda0-103">Get chatMessageHostedContent</span></span>

<span data-ttu-id="cbda0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cbda0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cbda0-105">Recupere as propriedades e os relacionamentos do objeto [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) .</span><span class="sxs-lookup"><span data-stu-id="cbda0-105">Retrieve the properties and relationships of [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="cbda0-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="cbda0-106">Permissions</span></span>

<span data-ttu-id="cbda0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cbda0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cbda0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cbda0-109">Permission type</span></span>                        | <span data-ttu-id="cbda0-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cbda0-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="cbda0-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cbda0-111">Delegated (work or school account)</span></span>| <span data-ttu-id="cbda0-112">Para recurso de **usuário** ou **chat** : chat. Read, chat. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cbda0-112">For **user** or **chat** resource: Chat.Read, Chat.ReadWrite</span></span><br/><br/><span data-ttu-id="cbda0-113">Para recurso de **canal** : ChannelMessage. Read. All, Group. Read. All, Group. Read. WriteAll</span><span class="sxs-lookup"><span data-stu-id="cbda0-113">For **channel** resource: ChannelMessage.Read.All, Group.Read.All, Group.Read.WriteAll</span></span> |
|<span data-ttu-id="cbda0-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cbda0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cbda0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cbda0-115">Not supported.</span></span>|
|<span data-ttu-id="cbda0-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cbda0-116">Application</span></span>| <span data-ttu-id="cbda0-117">Para o **usuário** ou recurso de **chat** : chat. Read. All, chat. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="cbda0-117">For **user** or **chat** resource: Chat.Read.All, Chat.ReadWrite.All</span></span><br/><br/><span data-ttu-id="cbda0-118">Para recurso de **canal** : ChannelMessage. Read. Group \*, ChannelMessage. Read. All, Group. Read. All, Group. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="cbda0-118">For **channel** resource: ChannelMessage.Read.Group\*, ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> |

> <span data-ttu-id="cbda0-119">**Observação**: as permissões marcadas com \* usam o [consentimento específico do recurso]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="cbda0-119">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> [!NOTE]
> <span data-ttu-id="cbda0-120">É necessário solicitar acesso antes de chamar essa API com permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="cbda0-120">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="cbda0-121">Para obter detalhes, confira [APIs protegidas no Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="cbda0-121">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="cbda0-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cbda0-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /chats/{id}/messages/{id}/hostedContents/{id}
GET /users/{id}/chats/{id}/messages/{id}/hostedContents/{id}
GET /teams/{id}/channels/{id}/messages/{id}/hostedContents/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cbda0-123">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="cbda0-123">Optional query parameters</span></span>

<span data-ttu-id="cbda0-124">Esta operação não é compatível com os [parâmetros de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="cbda0-124">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cbda0-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cbda0-125">Request headers</span></span>

| <span data-ttu-id="cbda0-126">Nome</span><span class="sxs-lookup"><span data-stu-id="cbda0-126">Name</span></span>      |<span data-ttu-id="cbda0-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="cbda0-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="cbda0-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="cbda0-128">Authorization</span></span> | <span data-ttu-id="cbda0-129">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="cbda0-129">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="cbda0-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cbda0-130">Request body</span></span>

<span data-ttu-id="cbda0-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cbda0-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cbda0-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="cbda0-132">Response</span></span>

<span data-ttu-id="cbda0-133">Se tiver êxito, este método retornará um `200 OK` código de resposta e o objeto [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cbda0-133">If successful, this method returns a `200 OK` response code and the requested [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cbda0-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="cbda0-134">Examples</span></span>

### <a name="example-1-get-hosted-content"></a><span data-ttu-id="cbda0-135">Exemplo 1: obter conteúdo hospedado</span><span class="sxs-lookup"><span data-stu-id="cbda0-135">Example 1: Get hosted content</span></span>

#### <a name="request"></a><span data-ttu-id="cbda0-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cbda0-136">Request</span></span>

<span data-ttu-id="cbda0-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="cbda0-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cbda0-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="cbda0-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chatmessagehostedcontent"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/chats/{id}/messages/{id}/hostedContents/{id}
```
# <a name="c"></a>[<span data-ttu-id="cbda0-139">C#</span><span class="sxs-lookup"><span data-stu-id="cbda0-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chatmessagehostedcontent-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cbda0-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cbda0-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chatmessagehostedcontent-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cbda0-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cbda0-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chatmessagehostedcontent-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="cbda0-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="cbda0-142">Response</span></span>

<span data-ttu-id="cbda0-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="cbda0-143">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="cbda0-144">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="cbda0-144">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="cbda0-145">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cbda0-145">All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-hosted-content-bytes-for-an-image"></a><span data-ttu-id="cbda0-146">Exemplo 2: obter bytes de conteúdo hospedados para uma imagem</span><span class="sxs-lookup"><span data-stu-id="cbda0-146">Example 2: Get hosted content bytes for an image</span></span>

#### <a name="request"></a><span data-ttu-id="cbda0-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cbda0-147">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="cbda0-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="cbda0-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chatmessagehostedcontent"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/chats/{id}/messages/{id}/hostedContents/{id}/$value
```
# <a name="c"></a>[<span data-ttu-id="cbda0-149">C#</span><span class="sxs-lookup"><span data-stu-id="cbda0-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chatmessagehostedcontent-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cbda0-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cbda0-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chatmessagehostedcontent-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cbda0-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cbda0-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chatmessagehostedcontent-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="cbda0-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="cbda0-152">Response</span></span>

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
