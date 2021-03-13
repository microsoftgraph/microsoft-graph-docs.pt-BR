---
title: Obtenha o conversationMember em um bate-papo.
description: Recuperar um membro de um bate-papo.
author: bhartono
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: b24b302565c62ee4a422d753160431099a81342d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50777570"
---
# <a name="get-conversationmember-in-a-chat"></a><span data-ttu-id="1e3bd-103">Obtenha o conversationMember em um bate-papo.</span><span class="sxs-lookup"><span data-stu-id="1e3bd-103">Get conversationMember in a chat</span></span>

<span data-ttu-id="1e3bd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1e3bd-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1e3bd-105">Recuperar um [conversationMember](../resources/conversationmember.md) de um [bate-papo](../resources/chat.md).</span><span class="sxs-lookup"><span data-stu-id="1e3bd-105">Retrieve a [conversationMember](../resources/conversationmember.md) from a [chat](../resources/chat.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1e3bd-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1e3bd-106">Permissions</span></span>

<span data-ttu-id="1e3bd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1e3bd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e3bd-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1e3bd-109">Permission Type</span></span>|<span data-ttu-id="1e3bd-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1e3bd-110">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="1e3bd-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1e3bd-111">Delegated (work or school account)</span></span>| <span data-ttu-id="1e3bd-112">ChatMember.Read, ChatMember.ReadWrite, Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1e3bd-112">ChatMember.Read, ChatMember.ReadWrite, Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span></span> |
|<span data-ttu-id="1e3bd-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1e3bd-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1e3bd-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1e3bd-114">Not supported.</span></span>|
|<span data-ttu-id="1e3bd-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1e3bd-115">Application</span></span>| <span data-ttu-id="1e3bd-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1e3bd-116">Not supported.</span></span> |

> <span data-ttu-id="1e3bd-117">**Observação**: Permissões marcadas com \* usam [consentimento específico de recurso](https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="1e3bd-117">**Note**: Permissions marked with \* use [resource-specific consent](https://aka.ms/teams-rsc).</span></span>

> [!NOTE]
> <span data-ttu-id="1e3bd-118">É necessário solicitar acesso antes de chamar essa API com permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1e3bd-118">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="1e3bd-119">Para obter detalhes, confira [APIs protegidas no Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="1e3bd-119">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="1e3bd-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1e3bd-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /chats/{chat-id}/members/{membership-id}
GET /users/{user-id}/chats/{chat-id}/members/{membership-id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1e3bd-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1e3bd-121">Optional query parameters</span></span>

<span data-ttu-id="1e3bd-122">Esta operação não é compatível com os [parâmetros de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1e3bd-122">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1e3bd-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1e3bd-123">Request headers</span></span>

| <span data-ttu-id="1e3bd-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1e3bd-124">Header</span></span>       | <span data-ttu-id="1e3bd-125">Valor</span><span class="sxs-lookup"><span data-stu-id="1e3bd-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1e3bd-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="1e3bd-126">Authorization</span></span>  | <span data-ttu-id="1e3bd-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1e3bd-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1e3bd-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1e3bd-129">Request body</span></span>

<span data-ttu-id="1e3bd-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1e3bd-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1e3bd-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="1e3bd-131">Response</span></span>

<span data-ttu-id="1e3bd-132">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [conversationMember](../resources/conversationmember.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1e3bd-132">If successful, this method returns a `200 OK` response code and a [conversationMember](../resources/conversationmember.md) object in the response body.</span></span>

> [!NOTE]
> <span data-ttu-id="1e3bd-133">Há alguns problemas conhecidos com essa funcionalidade.</span><span class="sxs-lookup"><span data-stu-id="1e3bd-133">There are some known issues with this functionality.</span></span> <span data-ttu-id="1e3bd-134">Para saber mais, confira [problemas conhecidos](/graph/known-issues#missing-properties-for-chat-members).</span><span class="sxs-lookup"><span data-stu-id="1e3bd-134">For details, see [known issues](/graph/known-issues#missing-properties-for-chat-members).</span></span>

## <a name="example"></a><span data-ttu-id="1e3bd-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1e3bd-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="1e3bd-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1e3bd-136">Request</span></span>

<span data-ttu-id="1e3bd-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1e3bd-137">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_conversation_member"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/chats/19:cf66807577b149cca1b7af0c32eec122@thread.v2/members/141c574c-dd90-4131-b173-baf4bb0e894e
```


### <a name="response"></a><span data-ttu-id="1e3bd-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="1e3bd-138">Response</span></span>

<span data-ttu-id="1e3bd-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1e3bd-139">Here is an example of the response.</span></span>

><span data-ttu-id="1e3bd-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1e3bd-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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


