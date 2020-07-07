---
title: Obter conversationMember
description: Recuperar um membro de um chat ou canal.
author: clearab
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 73f89ac24bedad9cfd632674040b288aac151f23
ms.sourcegitcommit: 67433748b69541727185fc1f32ed356718bf6ff1
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2020
ms.locfileid: "45050740"
---
# <a name="get-conversationmember"></a><span data-ttu-id="8ed0e-103">Obter conversationMember</span><span class="sxs-lookup"><span data-stu-id="8ed0e-103">Get conversationMember</span></span>

<span data-ttu-id="8ed0e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8ed0e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8ed0e-105">Recuperar um [conversationMember](../resources/conversationmember.md) de um [chat](../resources/chat.md) ou [canal](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="8ed0e-105">Retrieve a [conversationMember](../resources/conversationmember.md) from a [chat](../resources/chat.md) or [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8ed0e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="8ed0e-106">Permissions</span></span>

<span data-ttu-id="8ed0e-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="8ed0e-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="8ed0e-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8ed0e-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8ed0e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8ed0e-109">Permission Type</span></span>|<span data-ttu-id="8ed0e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8ed0e-110">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="8ed0e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8ed0e-111">Delegated (work or school account)</span></span>| <span data-ttu-id="8ed0e-112">Para o **usuário** ou recurso de **chat** : chat. ReadBasic, chat. Read, chat. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8ed0e-112">For **user** or **chat** resource: Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span></span><br/><br/><span data-ttu-id="8ed0e-113">Para recurso de **canal** : ChannelMember. Read. All, ChannelMember. ReadWrite, Group. Read. All, Group. ReadWrite. All, Directory. Read. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="8ed0e-113">For **channel** resource: ChannelMember.Read.All, ChannelMember.ReadWrite, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="8ed0e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8ed0e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8ed0e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8ed0e-115">Not supported.</span></span>|
|<span data-ttu-id="8ed0e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8ed0e-116">Application</span></span>| <span data-ttu-id="8ed0e-117">Para o **usuário** ou recurso de **chat** : chat. ReadBasic. All, chat. Read. All, chat. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="8ed0e-117">For **user** or **chat** resource: Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span></span><br/><br/><span data-ttu-id="8ed0e-118">Para o recurso de **canal** : member. Read. Group \*, ChannelMember. Read. All, ChannelMember. ReadWrite. All, Group. Read. All, Group. ReadWrite. All, Directory. Read. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="8ed0e-118">For **channel** resource: Member.Read.Group\*, ChannelMember.Read.All, ChannelMember.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="8ed0e-119">**Observação**: as permissões marcadas com \* usam o [consentimento específico do recurso](https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="8ed0e-119">**Note**: Permissions marked with \* use [resource-specific consent](https://aka.ms/teams-rsc).</span></span>

> [!NOTE]
> <span data-ttu-id="8ed0e-120">É necessário solicitar acesso antes de chamar essa API com permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8ed0e-120">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="8ed0e-121">Para obter detalhes, confira [APIs protegidas no Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="8ed0e-121">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="8ed0e-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8ed0e-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /chats/{id}/members/{id}
GET /users/{id}/chats/{id}/members/{id}
GET /teams/{id}/channels/{id}/members/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8ed0e-123">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8ed0e-123">Optional query parameters</span></span>

<span data-ttu-id="8ed0e-124">Esta operação não é compatível com os [parâmetros de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8ed0e-124">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8ed0e-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8ed0e-125">Request headers</span></span>

| <span data-ttu-id="8ed0e-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8ed0e-126">Header</span></span>       | <span data-ttu-id="8ed0e-127">Valor</span><span class="sxs-lookup"><span data-stu-id="8ed0e-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8ed0e-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="8ed0e-128">Authorization</span></span>  | <span data-ttu-id="8ed0e-129">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="8ed0e-129">Bearer {token}.</span></span> <span data-ttu-id="8ed0e-130">Required.</span><span class="sxs-lookup"><span data-stu-id="8ed0e-130">Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8ed0e-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8ed0e-131">Request body</span></span>

<span data-ttu-id="8ed0e-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8ed0e-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8ed0e-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="8ed0e-133">Response</span></span>

<span data-ttu-id="8ed0e-134">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [conversationMember](../resources/conversationmember.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8ed0e-134">If successful, this method returns a `200 OK` response code and a [conversationMember](../resources/conversationmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8ed0e-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8ed0e-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="8ed0e-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8ed0e-136">Request</span></span>

<span data-ttu-id="8ed0e-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8ed0e-137">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8ed0e-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="8ed0e-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_conversation_member"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/chats/{id}/members/{id}
```
# <a name="c"></a>[<span data-ttu-id="8ed0e-139">C#</span><span class="sxs-lookup"><span data-stu-id="8ed0e-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-conversation-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8ed0e-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8ed0e-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-conversation-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8ed0e-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8ed0e-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-conversation-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="8ed0e-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="8ed0e-142">Response</span></span>

<span data-ttu-id="8ed0e-143">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8ed0e-143">Here is an example of the response.</span></span>

><span data-ttu-id="8ed0e-144">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="8ed0e-144">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="8ed0e-145">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="8ed0e-145">All the properties will be returned from an actual call.</span></span>
<!-- {
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
