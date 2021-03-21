---
title: Obter conversationMember
description: Obtenha um membro do bate-papo ou do canal.
author: laujan
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 054bbb8d69d843fd26644ac658bd2b7553600a7a
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50963866"
---
# <a name="get-conversationmember"></a><span data-ttu-id="927a9-103">Obter conversationMember</span><span class="sxs-lookup"><span data-stu-id="927a9-103">Get conversationMember</span></span>

<span data-ttu-id="927a9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="927a9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="927a9-105">Recuperar um [conversationMember](../resources/conversationmember.md) de um [chat](../resources/chatmessage.md) ou [canal](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="927a9-105">Retrieve a [conversationMember](../resources/conversationmember.md) from a [chat](../resources/chatmessage.md) or [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="927a9-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="927a9-106">Permissions</span></span>

<span data-ttu-id="927a9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="927a9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="927a9-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="927a9-109">Permission Type</span></span>|<span data-ttu-id="927a9-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="927a9-110">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="927a9-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="927a9-111">Delegated (work or school account)</span></span>| <span data-ttu-id="927a9-112">Para recurso de **usuário** ou **chat**: Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="927a9-112">For **user** or **chat** resource: Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span></span><br/><br/><span data-ttu-id="927a9-113">Para o recurso **canal**: ChannelMember.Read.All, ChannelMember.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="927a9-113">For **channel** resource: ChannelMember.Read.All, ChannelMember.ReadWrite</span></span> |
|<span data-ttu-id="927a9-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="927a9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="927a9-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="927a9-115">Not supported.</span></span>|
|<span data-ttu-id="927a9-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="927a9-116">Application</span></span>| <span data-ttu-id="927a9-117">Para **usuário** ou **recurso de chat**: Não suportado.</span><span class="sxs-lookup"><span data-stu-id="927a9-117">For **user** or **chat** resource: Not supported.</span></span><br/><br/><span data-ttu-id="927a9-118">Para o recurso **canal**: TeamMember.Read.Group\*, ChannelMember.Read.All, ChannelMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="927a9-118">For **channel** resource: TeamMember.Read.Group\*, ChannelMember.Read.All, ChannelMember.ReadWrite.All</span></span> |

> <span data-ttu-id="927a9-119">**Observação**: Permissões marcadas com \* usam [consentimento específico de recurso](https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="927a9-119">**Note**: Permissions marked with \* use [resource-specific consent](https://aka.ms/teams-rsc).</span></span>

> [!NOTE]
> <span data-ttu-id="927a9-120">É necessário solicitar acesso antes de chamar essa API com permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="927a9-120">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="927a9-121">Para obter detalhes, confira [APIs protegidas no Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="927a9-121">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="927a9-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="927a9-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /chats/{id}/members/{id}
GET /teams/{id}/channels/{id}/members/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="927a9-123">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="927a9-123">Optional query parameters</span></span>

<span data-ttu-id="927a9-124">Esta operação não é compatível com os [parâmetros de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="927a9-124">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="927a9-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="927a9-125">Request headers</span></span>

| <span data-ttu-id="927a9-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="927a9-126">Header</span></span>       | <span data-ttu-id="927a9-127">Valor</span><span class="sxs-lookup"><span data-stu-id="927a9-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="927a9-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="927a9-128">Authorization</span></span>  | <span data-ttu-id="927a9-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="927a9-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="927a9-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="927a9-131">Request body</span></span>

<span data-ttu-id="927a9-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="927a9-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="927a9-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="927a9-133">Response</span></span>

<span data-ttu-id="927a9-134">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [conversationMember](../resources/conversationmember.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="927a9-134">If successful, this method returns a `200 OK` response code and a [conversationMember](../resources/conversationmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="927a9-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="927a9-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="927a9-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="927a9-136">Request</span></span>

<span data-ttu-id="927a9-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="927a9-137">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="927a9-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="927a9-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_conversation_member_2"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/V1.0/chats/{id}/members/{id}
```
# <a name="c"></a>[<span data-ttu-id="927a9-139">C#</span><span class="sxs-lookup"><span data-stu-id="927a9-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-conversation-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="927a9-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="927a9-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-conversation-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="927a9-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="927a9-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-conversation-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="927a9-142">Java</span><span class="sxs-lookup"><span data-stu-id="927a9-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-conversation-member-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="927a9-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="927a9-143">Response</span></span>

<span data-ttu-id="927a9-144">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="927a9-144">Here is an example of the response.</span></span>

><span data-ttu-id="927a9-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="927a9-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!--
{
  "blockType": "response",
  "truncated": true,
  "name": "get_conversation_member_2",
  "@odata.type": "microsoft.graph.conversationMember"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
  "id": "id-value",
  "displayName": "display-name-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "conversation: member get",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
