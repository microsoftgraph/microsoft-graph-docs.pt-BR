---
title: 'conversationMember: adicionar'
description: Adicionar membros em massa à equipe.
author: nkramer
doc_type: apiPageType
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: ffc3d9d36c0f4d22653a961ebe5af4769f286d7d
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/11/2020
ms.locfileid: "49658324"
---
# <a name="conversationmember-add"></a><span data-ttu-id="ab2af-103">conversationMember: adicionar</span><span class="sxs-lookup"><span data-stu-id="ab2af-103">conversationMember: add</span></span>

<span data-ttu-id="ab2af-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ab2af-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ab2af-105">Adicione vários membros em uma única solicitação a uma [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="ab2af-105">Add multiple members in a single request to a [team](../resources/team.md).</span></span> <span data-ttu-id="ab2af-106">A resposta fornece detalhes sobre quais associações podem e não podem ser criadas.</span><span class="sxs-lookup"><span data-stu-id="ab2af-106">The response provides details about which memberships could and could not be created.</span></span>

## <a name="permissions"></a><span data-ttu-id="ab2af-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="ab2af-107">Permissions</span></span>

<span data-ttu-id="ab2af-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ab2af-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ab2af-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ab2af-110">Permission type</span></span>      | <span data-ttu-id="ab2af-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ab2af-111">Permissions (from least to most privileged)</span></span> | 
|:--------------------|:--------------------------|
| <span data-ttu-id="ab2af-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ab2af-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ab2af-113">TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab2af-113">TeamMember.ReadWrite.All</span></span>  |
| <span data-ttu-id="ab2af-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ab2af-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ab2af-115">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="ab2af-115">Not supported</span></span> |
| <span data-ttu-id="ab2af-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ab2af-116">Application</span></span> | <span data-ttu-id="ab2af-117">TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab2af-117">TeamMember.ReadWrite.All</span></span>   |


## <a name="http-request"></a><span data-ttu-id="ab2af-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ab2af-118">HTTP Request</span></span>

<span data-ttu-id="ab2af-119">Esta é uma ação vinculada para adicionar vários elementos a uma coleção **chatMember** em uma única solicitação.</span><span class="sxs-lookup"><span data-stu-id="ab2af-119">This is a bound action for adding multiple elements to a **conversationMember** collection in a single request.</span></span>
<!-- { "blockType": "ignored" } -->

```http
POST /teams/{team-id}/members/add
```

## <a name="request-headers"></a><span data-ttu-id="ab2af-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ab2af-120">Request headers</span></span>

| <span data-ttu-id="ab2af-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ab2af-121">Header</span></span>        | <span data-ttu-id="ab2af-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ab2af-122">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="ab2af-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ab2af-123">Authorization</span></span> | <span data-ttu-id="ab2af-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ab2af-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ab2af-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ab2af-126">Request body</span></span>
<span data-ttu-id="ab2af-127">No corpo da solicitação, forneça a representação JSON da lista de `conversationMember` derivados que precisam ser adicionados à equipe.</span><span class="sxs-lookup"><span data-stu-id="ab2af-127">In the request body, supply the JSON representation of the list of `conversationMember` derivatives that need to be added to the team.</span></span>

<span data-ttu-id="ab2af-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="ab2af-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="ab2af-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="ab2af-129">Parameter</span></span>|<span data-ttu-id="ab2af-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="ab2af-130">Type</span></span>|<span data-ttu-id="ab2af-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="ab2af-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab2af-132">values</span><span class="sxs-lookup"><span data-stu-id="ab2af-132">values</span></span>|<span data-ttu-id="ab2af-133">coleção [conversationMember](../resources/conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="ab2af-133">[conversationMember](../resources/conversationmember.md) collection</span></span>|<span data-ttu-id="ab2af-134">Lista de membros da conversa que devem ser adicionados.</span><span class="sxs-lookup"><span data-stu-id="ab2af-134">List of conversation members that should be added.</span></span>|


## <a name="response"></a><span data-ttu-id="ab2af-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="ab2af-135">Response</span></span>

<span data-ttu-id="ab2af-136">Se bem-sucedida, esta ação retorna um código de resposta `200 OK`e uma coleção de derivados de [actionResultPart](../resources/actionresultpart.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ab2af-136">If successful, this action returns a `200 OK` response code and a collection of derivatives of [actionResultPart](../resources/actionresultpart.md) in the response body.</span></span>

<span data-ttu-id="ab2af-137">Esta API retorna uma resposta `200` indicando que todos os membros fornecidos foram adicionados à equipe ou uma resposta `207` indicando que apenas alguns dos membros fornecidos foram adicionados à equipe.</span><span class="sxs-lookup"><span data-stu-id="ab2af-137">This API returns a `200` response indicating all members supplied were added to the team or a `207` response indicating that only some of the supplied members were added to the team.</span></span> <span data-ttu-id="ab2af-138">O chamador deve inspecionar a carga útil de resposta para determinar quais adições de membro falharam.</span><span class="sxs-lookup"><span data-stu-id="ab2af-138">The caller should inspect the response payload to determine which member additions failed.</span></span> <span data-ttu-id="ab2af-139">O corpo da resposta é uma coleção de derivados do recurso [actionResultPart](../resources/actionresultpart.md).</span><span class="sxs-lookup"><span data-stu-id="ab2af-139">The response body is a collection of derivatives of the [actionResultPart](../resources/actionresultpart.md) resource.</span></span>

## <a name="examples"></a><span data-ttu-id="ab2af-140">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ab2af-140">Examples</span></span>

### <a name="example-1-add-members-in-bulk-to-a-team"></a><span data-ttu-id="ab2af-141">Exemplo 1: adicionar membros em massa a uma equipe</span><span class="sxs-lookup"><span data-stu-id="ab2af-141">Example 1: Add members in bulk to a team</span></span>

#### <a name="request"></a><span data-ttu-id="ab2af-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ab2af-142">Request</span></span>

<span data-ttu-id="ab2af-143">O exemplo a seguir mostra uma solicitação para adicionar vários membros a uma equipe.</span><span class="sxs-lookup"><span data-stu-id="ab2af-143">The following example shows a request to add multiple members to a team.</span></span>
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

#### <a name="response"></a><span data-ttu-id="ab2af-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="ab2af-144">Response</span></span>

<span data-ttu-id="ab2af-145">Esta é a resposta.</span><span class="sxs-lookup"><span data-stu-id="ab2af-145">The following is the response.</span></span>

> <span data-ttu-id="ab2af-146">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ab2af-146">**Note:** The response object shown here might be shortened for readability.</span></span> 
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

### <a name="example-2-add-members-in-bulk-and-encounter-partial-failure"></a><span data-ttu-id="ab2af-147">Exemplo 2: adicionar membros em massa e encontrar falha parcial</span><span class="sxs-lookup"><span data-stu-id="ab2af-147">Example 2: Add members in bulk and encounter partial failure</span></span>

#### <a name="request"></a><span data-ttu-id="ab2af-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ab2af-148">Request</span></span>

<span data-ttu-id="ab2af-149">O exemplo a seguir mostra uma solicitação para adicionar vários membros a uma equipe que resulta em uma falha parcial.</span><span class="sxs-lookup"><span data-stu-id="ab2af-149">The following example shows a request to add multiple members to a team that results in a partial failure.</span></span>

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

#### <a name="response"></a><span data-ttu-id="ab2af-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="ab2af-150">Response</span></span>

<span data-ttu-id="ab2af-151">Esta é a resposta.</span><span class="sxs-lookup"><span data-stu-id="ab2af-151">The following is the response.</span></span>

> <span data-ttu-id="ab2af-152">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ab2af-152">**Note:** The response object shown here might be shortened for readability.</span></span> 
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


## <a name="see-also"></a><span data-ttu-id="ab2af-153">Confira também</span><span class="sxs-lookup"><span data-stu-id="ab2af-153">See also</span></span>

- [<span data-ttu-id="ab2af-154">Adicionar membro à equipe</span><span class="sxs-lookup"><span data-stu-id="ab2af-154">Add member to team</span></span>](team-post-members.md)

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
