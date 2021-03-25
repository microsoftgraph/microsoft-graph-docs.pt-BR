---
title: Obtenha o conversationMember em um bate-papo.
description: Recuperar um membro de um bate-papo.
author: bhartono
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 9ef01b0308df8ffd05a6337b18c4f8c16a359114
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51202377"
---
# <a name="get-conversationmember-in-a-chat"></a><span data-ttu-id="e1fbd-103">Obtenha o conversationMember em um bate-papo.</span><span class="sxs-lookup"><span data-stu-id="e1fbd-103">Get conversationMember in a chat</span></span>

<span data-ttu-id="e1fbd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e1fbd-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e1fbd-105">Recuperar um [conversationMember](../resources/conversationmember.md) de um [bate-papo](../resources/chat.md).</span><span class="sxs-lookup"><span data-stu-id="e1fbd-105">Retrieve a [conversationMember](../resources/conversationmember.md) from a [chat](../resources/chat.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e1fbd-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e1fbd-106">Permissions</span></span>

<span data-ttu-id="e1fbd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1fbd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1fbd-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e1fbd-109">Permission Type</span></span>|<span data-ttu-id="e1fbd-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e1fbd-110">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="e1fbd-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e1fbd-111">Delegated (work or school account)</span></span>| <span data-ttu-id="e1fbd-112">ChatMember.Read, ChatMember.ReadWrite, Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e1fbd-112">ChatMember.Read, ChatMember.ReadWrite, Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span></span> |
|<span data-ttu-id="e1fbd-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e1fbd-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e1fbd-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e1fbd-114">Not supported.</span></span>|
|<span data-ttu-id="e1fbd-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e1fbd-115">Application</span></span>| <span data-ttu-id="e1fbd-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e1fbd-116">Not supported.</span></span> |

> <span data-ttu-id="e1fbd-117">**Observação**: Permissões marcadas com \* usam [consentimento específico de recurso](https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="e1fbd-117">**Note**: Permissions marked with \* use [resource-specific consent](https://aka.ms/teams-rsc).</span></span>

> [!NOTE]
> <span data-ttu-id="e1fbd-118">É necessário solicitar acesso antes de chamar essa API com permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e1fbd-118">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="e1fbd-119">Para obter detalhes, confira [APIs protegidas no Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="e1fbd-119">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="e1fbd-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e1fbd-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /chats/{chat-id}/members/{membership-id}
GET /users/{user-id}/chats/{chat-id}/members/{membership-id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e1fbd-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e1fbd-121">Optional query parameters</span></span>

<span data-ttu-id="e1fbd-122">Esta operação não é compatível com os [parâmetros de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e1fbd-122">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e1fbd-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e1fbd-123">Request headers</span></span>

| <span data-ttu-id="e1fbd-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e1fbd-124">Header</span></span>       | <span data-ttu-id="e1fbd-125">Valor</span><span class="sxs-lookup"><span data-stu-id="e1fbd-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e1fbd-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="e1fbd-126">Authorization</span></span>  | <span data-ttu-id="e1fbd-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e1fbd-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e1fbd-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e1fbd-129">Request body</span></span>

<span data-ttu-id="e1fbd-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e1fbd-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e1fbd-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1fbd-131">Response</span></span>

<span data-ttu-id="e1fbd-132">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [conversationMember](../resources/conversationmember.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e1fbd-132">If successful, this method returns a `200 OK` response code and a [conversationMember](../resources/conversationmember.md) object in the response body.</span></span>

> [!NOTE]
> <span data-ttu-id="e1fbd-133">Há alguns problemas conhecidos com essa funcionalidade.</span><span class="sxs-lookup"><span data-stu-id="e1fbd-133">There are some known issues with this functionality.</span></span> <span data-ttu-id="e1fbd-134">Para saber mais, confira [problemas conhecidos](/graph/known-issues#missing-properties-for-chat-members).</span><span class="sxs-lookup"><span data-stu-id="e1fbd-134">For details, see [known issues](/graph/known-issues#missing-properties-for-chat-members).</span></span>

## <a name="example"></a><span data-ttu-id="e1fbd-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e1fbd-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="e1fbd-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e1fbd-136">Request</span></span>

<span data-ttu-id="e1fbd-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e1fbd-137">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="e1fbd-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="e1fbd-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_conversation_member_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/chats/19:cf66807577b149cca1b7af0c32eec122@thread.v2/members/141c574c-dd90-4131-b173-baf4bb0e894e
```
# <a name="c"></a>[<span data-ttu-id="e1fbd-139">C#</span><span class="sxs-lookup"><span data-stu-id="e1fbd-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-conversation-member-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e1fbd-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e1fbd-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-conversation-member-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e1fbd-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e1fbd-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-conversation-member-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e1fbd-142">Java</span><span class="sxs-lookup"><span data-stu-id="e1fbd-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-conversation-member-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="e1fbd-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1fbd-143">Response</span></span>

<span data-ttu-id="e1fbd-144">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e1fbd-144">Here is an example of the response.</span></span>

><span data-ttu-id="e1fbd-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e1fbd-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- 
{
 "blockType": "response",
  "truncated": true,
  "name": "get_conversation_member_1",
  "@odata.type": "microsoft.graph.conversationMember"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
    "@odata.type": "#microsoft.graph.aadUserConversationMember",
    "id": "07ad17ad-ada5-4f1f-a650-7a963886a8a7",
    "roles": [ "owner" ],
    "displayName": "Minna Pham",
    "userId": "07ad17ad-ada5-4f1f-a650-7a963886a8a7",
    "email": null,
    "tenantId": "6e5147da-6a35-4275-b3f3-fc069456b6eb",
    "visibleHistoryStartDateTime": "2019-04-18T23:51:43.255Z"
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


