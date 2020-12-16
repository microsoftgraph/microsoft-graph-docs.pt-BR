---
title: 'conversationMember: adicionar'
description: Adicionar membros em massa à equipe.
author: nkramer
doc_type: apiPageType
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 2af435ac7dd430a0d006df609991f0c0a83b02ca
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/16/2020
ms.locfileid: "49689635"
---
# <a name="conversationmember-add"></a><span data-ttu-id="28871-103">conversationMember: adicionar</span><span class="sxs-lookup"><span data-stu-id="28871-103">conversationMember: add</span></span>

<span data-ttu-id="28871-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="28871-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="28871-105">Adicione vários membros em uma única solicitação a uma [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="28871-105">Add multiple members in a single request to a [team](../resources/team.md).</span></span> <span data-ttu-id="28871-106">A resposta fornece detalhes sobre quais associações podem e não podem ser criadas.</span><span class="sxs-lookup"><span data-stu-id="28871-106">The response provides details about which memberships could and could not be created.</span></span>

## <a name="permissions"></a><span data-ttu-id="28871-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="28871-107">Permissions</span></span>

<span data-ttu-id="28871-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="28871-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="28871-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="28871-110">Permission type</span></span>      | <span data-ttu-id="28871-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="28871-111">Permissions (from least to most privileged)</span></span> | 
|:--------------------|:--------------------------|
| <span data-ttu-id="28871-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="28871-112">Delegated (work or school account)</span></span> | <span data-ttu-id="28871-113">TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28871-113">TeamMember.ReadWrite.All</span></span>  |
| <span data-ttu-id="28871-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="28871-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="28871-115">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="28871-115">Not supported</span></span> |
| <span data-ttu-id="28871-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="28871-116">Application</span></span> | <span data-ttu-id="28871-117">TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28871-117">TeamMember.ReadWrite.All</span></span>   |


## <a name="http-request"></a><span data-ttu-id="28871-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="28871-118">HTTP Request</span></span>

<span data-ttu-id="28871-119">Esta é uma ação vinculada para adicionar vários elementos a uma coleção **chatMember** em uma única solicitação.</span><span class="sxs-lookup"><span data-stu-id="28871-119">This is a bound action for adding multiple elements to a **conversationMember** collection in a single request.</span></span>
<!-- { "blockType": "ignored" } -->

```http
POST /teams/{team-id}/members/add
```

## <a name="request-headers"></a><span data-ttu-id="28871-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="28871-120">Request headers</span></span>

| <span data-ttu-id="28871-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="28871-121">Header</span></span>        | <span data-ttu-id="28871-122">Valor</span><span class="sxs-lookup"><span data-stu-id="28871-122">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="28871-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="28871-123">Authorization</span></span> | <span data-ttu-id="28871-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="28871-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="28871-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="28871-126">Request body</span></span>
<span data-ttu-id="28871-127">No corpo da solicitação, forneça a representação JSON da lista de `conversationMember` derivados que precisam ser adicionados à equipe.</span><span class="sxs-lookup"><span data-stu-id="28871-127">In the request body, supply the JSON representation of the list of `conversationMember` derivatives that need to be added to the team.</span></span>

<span data-ttu-id="28871-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="28871-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="28871-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="28871-129">Parameter</span></span>|<span data-ttu-id="28871-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="28871-130">Type</span></span>|<span data-ttu-id="28871-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="28871-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="28871-132">values</span><span class="sxs-lookup"><span data-stu-id="28871-132">values</span></span>|<span data-ttu-id="28871-133">coleção [conversationMember](../resources/conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="28871-133">[conversationMember](../resources/conversationmember.md) collection</span></span>|<span data-ttu-id="28871-134">Lista de membros da conversa que devem ser adicionados.</span><span class="sxs-lookup"><span data-stu-id="28871-134">List of conversation members that should be added.</span></span>|


## <a name="response"></a><span data-ttu-id="28871-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="28871-135">Response</span></span>

<span data-ttu-id="28871-136">Se bem-sucedida, esta ação retorna um código de resposta `200 OK`e uma coleção de derivados de [actionResultPart](../resources/actionresultpart.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="28871-136">If successful, this action returns a `200 OK` response code and a collection of derivatives of [actionResultPart](../resources/actionresultpart.md) in the response body.</span></span>

<span data-ttu-id="28871-137">Esta API retorna uma resposta `200` indicando que todos os membros fornecidos foram adicionados à equipe ou uma resposta `207` indicando que apenas alguns dos membros fornecidos foram adicionados à equipe.</span><span class="sxs-lookup"><span data-stu-id="28871-137">This API returns a `200` response indicating all members supplied were added to the team or a `207` response indicating that only some of the supplied members were added to the team.</span></span> <span data-ttu-id="28871-138">O chamador deve inspecionar a carga útil de resposta para determinar quais adições de membro falharam.</span><span class="sxs-lookup"><span data-stu-id="28871-138">The caller should inspect the response payload to determine which member additions failed.</span></span> <span data-ttu-id="28871-139">O corpo da resposta é uma coleção de derivados do recurso [actionResultPart](../resources/actionresultpart.md).</span><span class="sxs-lookup"><span data-stu-id="28871-139">The response body is a collection of derivatives of the [actionResultPart](../resources/actionresultpart.md) resource.</span></span>

## <a name="examples"></a><span data-ttu-id="28871-140">Exemplos</span><span class="sxs-lookup"><span data-stu-id="28871-140">Examples</span></span>

### <a name="example-1-add-members-in-bulk-to-a-team"></a><span data-ttu-id="28871-141">Exemplo 1: adicionar membros em massa a uma equipe</span><span class="sxs-lookup"><span data-stu-id="28871-141">Example 1: Add members in bulk to a team</span></span>

#### <a name="request"></a><span data-ttu-id="28871-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="28871-142">Request</span></span>

<span data-ttu-id="28871-143">O exemplo a seguir mostra uma solicitação para adicionar vários membros a uma equipe.</span><span class="sxs-lookup"><span data-stu-id="28871-143">The following example shows a request to add multiple members to a team.</span></span>

# <a name="http"></a>[<span data-ttu-id="28871-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="28871-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "bulkaddmembers_team"
}-->

```http
POST https://graph.microsoft.com/beta/teams/e4183b04-c9a2-417c-bde4-70e3ee46a6dc/members/add
Content-Type: application/json

{
    "values": [
        {
            "@odata.type": "microsoft.graph.aadUserConversationMember",
            "roles":[],
            "user@odata.bind": "https://graph.microsoft.com/beta/users('18a80140-b0fb-4489-b360-2f6efaf225a0')"
        },
        {
            "@odata.type": "microsoft.graph.aadUserConversationMember",
            "roles":["owner"],
            "user@odata.bind": "https://graph.microsoft.com/beta/users('86503198-b81b-43fe-81ee-ad45b8848ac9')"
        }
    ]
}
```
# <a name="c"></a>[<span data-ttu-id="28871-145">C#</span><span class="sxs-lookup"><span data-stu-id="28871-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/bulkaddmembers-team-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="28871-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="28871-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/bulkaddmembers-team-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="28871-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="28871-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/bulkaddmembers-team-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="28871-148">Java</span><span class="sxs-lookup"><span data-stu-id="28871-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/bulkaddmembers-team-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="28871-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="28871-149">Response</span></span>

<span data-ttu-id="28871-150">Esta é a resposta.</span><span class="sxs-lookup"><span data-stu-id="28871-150">The following is the response.</span></span>

> <span data-ttu-id="28871-151">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="28871-151">**Note:** The response object shown here might be shortened for readability.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.actionResultPart)"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.aadUserConversationMemberResult)",
    "value": [
        {
            "@odata.type": "#microsoft.graph.aadUserConversationMemberResult",
            "userId": "18a80140-b0fb-4489-b360-2f6efaf225a0",
            "error": null
        },
        {
            "@odata.type": "#microsoft.graph.aadUserConversationMemberResult",
            "userId": "86503198-b81b-43fe-81ee-ad45b8848ac9",
            "error": null
        }
    ]
}
```

### <a name="example-2-add-members-in-bulk-and-encounter-partial-failure"></a><span data-ttu-id="28871-152">Exemplo 2: adicionar membros em massa e encontrar falha parcial</span><span class="sxs-lookup"><span data-stu-id="28871-152">Example 2: Add members in bulk and encounter partial failure</span></span>

#### <a name="request"></a><span data-ttu-id="28871-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="28871-153">Request</span></span>

<span data-ttu-id="28871-154">O exemplo a seguir mostra uma solicitação para adicionar vários membros a uma equipe que resulta em uma falha parcial.</span><span class="sxs-lookup"><span data-stu-id="28871-154">The following example shows a request to add multiple members to a team that results in a partial failure.</span></span>


# <a name="http"></a>[<span data-ttu-id="28871-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="28871-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "bulkaddmembers_team_partial_failure"
}-->

```http
POST https://graph.microsoft.com/beta/teams/e4183b04-c9a2-417c-bde4-70e3ee46a6dc/members/add
Content-Type: application/json

{
    "values": [
        {
            "@odata.type": "microsoft.graph.aadUserConversationMember",
            "roles":[],
            "user@odata.bind": "https://graph.microsoft.com/beta/users('18a80140-b0fb-4489-b360-2f6efaf225a0')"
        },
        {
            "@odata.type": "microsoft.graph.aadUserConversationMember",
            "roles":["owner"],
            "user@odata.bind": "https://graph.microsoft.com/beta/users('86503198-b81b-43fe-81ee-ad45b8848ac9')"
        }
    ]
}
```
# <a name="c"></a>[<span data-ttu-id="28871-156">C#</span><span class="sxs-lookup"><span data-stu-id="28871-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/bulkaddmembers-team-partial-failure-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="28871-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="28871-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/bulkaddmembers-team-partial-failure-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="28871-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="28871-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/bulkaddmembers-team-partial-failure-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="28871-159">Java</span><span class="sxs-lookup"><span data-stu-id="28871-159">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/bulkaddmembers-team-partial-failure-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="28871-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="28871-160">Response</span></span>

<span data-ttu-id="28871-161">Esta é a resposta.</span><span class="sxs-lookup"><span data-stu-id="28871-161">The following is the response.</span></span>

> <span data-ttu-id="28871-162">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="28871-162">**Note:** The response object shown here might be shortened for readability.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.actionResultPart)"
} -->

```http
HTTP/1.1 207 MULTI-STATUS
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.addConversationMemberResult)",
    "value": [
        {
            "@odata.type": "#microsoft.graph.aadUserConversationMemberResult",
            "userId": "18a80140-b0fb-4489-b360-2f6efaf225a0",
            "error": {
                "code": "NotFound",
                "message": ""
            }
        },
        {
            "@odata.type": "#microsoft.graph.aadUserConversationMemberResult",
            "userId": "86503198-b81b-43fe-81ee-ad45b8848ac9",
            "error": null
        }
    ]
}
```


## <a name="see-also"></a><span data-ttu-id="28871-163">Confira também</span><span class="sxs-lookup"><span data-stu-id="28871-163">See also</span></span>

- [<span data-ttu-id="28871-164">Adicionar membro à equipe</span><span class="sxs-lookup"><span data-stu-id="28871-164">Add member to team</span></span>](team-post-members.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Add members to team in bulk",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
