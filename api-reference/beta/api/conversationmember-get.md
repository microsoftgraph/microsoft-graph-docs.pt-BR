---
title: Obter conversationMember
description: Recuperar um membro de um chat ou canal.
author: clearab
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 3e8e8e37b2c94a5ee41bf1bb4dc30adf30974166
ms.sourcegitcommit: 6201b3a5646f640f25a68ab033eca9eb60ccd05e
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/21/2020
ms.locfileid: "49376925"
---
# <a name="get-conversationmember"></a><span data-ttu-id="ebdec-103">Obter conversationMember</span><span class="sxs-lookup"><span data-stu-id="ebdec-103">Get conversationMember</span></span>

<span data-ttu-id="ebdec-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ebdec-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ebdec-105">Recuperar um [conversationMember](../resources/conversationmember.md) de um [chat](../resources/chat.md) ou [canal](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="ebdec-105">Retrieve a [conversationMember](../resources/conversationmember.md) from a [chat](../resources/chat.md) or [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ebdec-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ebdec-106">Permissions</span></span>

<span data-ttu-id="ebdec-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ebdec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ebdec-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ebdec-109">Permission Type</span></span>|<span data-ttu-id="ebdec-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ebdec-110">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="ebdec-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ebdec-111">Delegated (work or school account)</span></span>| <span data-ttu-id="ebdec-112">Para recurso de **usuário** ou **chat**: Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ebdec-112">For **user** or **chat** resource: Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span></span><br/><br/><span data-ttu-id="ebdec-113">Para recurso de **canal**: ChannelMember.Read.All, ChannelMember.ReadWrite, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory. ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ebdec-113">For **channel** resource: ChannelMember.Read.All, ChannelMember.ReadWrite, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="ebdec-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ebdec-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ebdec-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ebdec-115">Not supported.</span></span>|
|<span data-ttu-id="ebdec-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ebdec-116">Application</span></span>| <span data-ttu-id="ebdec-117">Para **usuário** ou **recurso de chat**: Não suportado.</span><span class="sxs-lookup"><span data-stu-id="ebdec-117">For **user** or **chat** resource: Not supported.</span></span><br/><br/><span data-ttu-id="ebdec-118">Para recurso de **canal**: Member.Read.Group\*, ChannelMember.Read.All, ChannelMember.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ebdec-118">For **channel** resource: Member.Read.Group\*, ChannelMember.Read.All, ChannelMember.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="ebdec-119">**Observação**: Permissões marcadas com \* usam [consentimento específico de recurso](https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="ebdec-119">**Note**: Permissions marked with \* use [resource-specific consent](https://aka.ms/teams-rsc).</span></span>

> [!NOTE]
> <span data-ttu-id="ebdec-p102">Before calling this API with application permissions, you must request access. For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="ebdec-p102">Before calling this API with application permissions, you must request access. For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="ebdec-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ebdec-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /chats/{id}/members/{id}
GET /users/{id}/chats/{id}/members/{id}
GET /teams/{id}/channels/{id}/members/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ebdec-123">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ebdec-123">Optional query parameters</span></span>

<span data-ttu-id="ebdec-124">Esta operação não é compatível com os [parâmetros de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ebdec-124">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ebdec-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ebdec-125">Request headers</span></span>

| <span data-ttu-id="ebdec-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ebdec-126">Header</span></span>       | <span data-ttu-id="ebdec-127">Valor</span><span class="sxs-lookup"><span data-stu-id="ebdec-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ebdec-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="ebdec-128">Authorization</span></span>  | <span data-ttu-id="ebdec-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ebdec-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ebdec-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ebdec-131">Request body</span></span>

<span data-ttu-id="ebdec-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ebdec-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ebdec-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="ebdec-133">Response</span></span>

<span data-ttu-id="ebdec-134">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [conversationMember](../resources/conversationmember.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ebdec-134">If successful, this method returns a `200 OK` response code and a [conversationMember](../resources/conversationmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ebdec-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ebdec-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="ebdec-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ebdec-136">Request</span></span>

<span data-ttu-id="ebdec-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ebdec-137">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ebdec-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="ebdec-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_conversation_member"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/chats/{id}/members/{id}
```
# <a name="c"></a>[<span data-ttu-id="ebdec-139">C#</span><span class="sxs-lookup"><span data-stu-id="ebdec-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-conversation-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ebdec-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ebdec-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-conversation-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ebdec-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ebdec-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-conversation-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ebdec-142">Java</span><span class="sxs-lookup"><span data-stu-id="ebdec-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-conversation-member-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="ebdec-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="ebdec-143">Response</span></span>

<span data-ttu-id="ebdec-144">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ebdec-144">Here is an example of the response.</span></span>

><span data-ttu-id="ebdec-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ebdec-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- 
{
 "blockType": "response",
  "truncated": true,
  "name": "get_conversation_member",
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


