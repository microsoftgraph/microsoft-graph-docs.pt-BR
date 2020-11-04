---
title: Listar membros
description: Obtenha o conversationMembers de uma equipe.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 9ff0912caecb5947e18d05ae5c7f3b36b571a158
ms.sourcegitcommit: d1e72c8d36aad78732133f9ecefaf66c433b8530
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2020
ms.locfileid: "48848623"
---
# <a name="list-members"></a><span data-ttu-id="278a7-103">Listar membros</span><span class="sxs-lookup"><span data-stu-id="278a7-103">List members</span></span>
<span data-ttu-id="278a7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="278a7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="278a7-105">Obtenha o [conversationMember](../resources/conversationmember.md) de uma [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="278a7-105">Get the [conversationMember](../resources/conversationmember.md) of a [team](../resources/team.md).</span></span>

><span data-ttu-id="278a7-106">Observação: atualmente, esta API não é compatível com a paginação, portanto, se houver muitos membros para se ajustarem a uma solicitação, você não terá todos os membros.</span><span class="sxs-lookup"><span data-stu-id="278a7-106">Note: This API currently does not support pagination, so if there's too many members to fit into one request, you won't get all the members.</span></span>

## <a name="permissions"></a><span data-ttu-id="278a7-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="278a7-107">Permissions</span></span>
<span data-ttu-id="278a7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="278a7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="278a7-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="278a7-110">Permission type</span></span>|<span data-ttu-id="278a7-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="278a7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="278a7-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="278a7-112">Delegated (work or school account)</span></span>| <span data-ttu-id="278a7-113">TeamMember.Read.All, TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="278a7-113">TeamMember.Read.All, TeamMember.ReadWrite.All</span></span> |
|<span data-ttu-id="278a7-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="278a7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="278a7-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="278a7-115">Not supported.</span></span>    |
|<span data-ttu-id="278a7-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="278a7-116">Application</span></span>| <span data-ttu-id="278a7-117">TeamMember.Read.All, TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="278a7-117">TeamMember.Read.All, TeamMember.ReadWrite.All</span></span> |

> <span data-ttu-id="278a7-118">**Observação** : Permissões marcadas com \* usam [consentimento específico de recurso]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="278a7-118">**Note** : Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

## <a name="http-request"></a><span data-ttu-id="278a7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="278a7-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /teams/{teamsId}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="278a7-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="278a7-120">Optional query parameters</span></span>
<span data-ttu-id="278a7-121">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="278a7-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="278a7-122">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="278a7-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="278a7-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="278a7-123">Request headers</span></span>
|<span data-ttu-id="278a7-124">Nome</span><span class="sxs-lookup"><span data-stu-id="278a7-124">Name</span></span>|<span data-ttu-id="278a7-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="278a7-125">Description</span></span>|
|:---|:---|
|<span data-ttu-id="278a7-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="278a7-126">Authorization</span></span>|<span data-ttu-id="278a7-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="278a7-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="278a7-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="278a7-129">Request body</span></span>
<span data-ttu-id="278a7-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="278a7-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="278a7-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="278a7-131">Response</span></span>

<span data-ttu-id="278a7-132">Se bem sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [conversationMember](../resources/conversationmember.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="278a7-132">If successful, this method returns a `200 OK` response code and a collection of [conversationMember](../resources/conversationmember.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="278a7-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="278a7-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="278a7-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="278a7-134">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="278a7-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="278a7-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_conversationmember"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/teams/{teamsId}/members
```
# <a name="c"></a>[<span data-ttu-id="278a7-136">C#</span><span class="sxs-lookup"><span data-stu-id="278a7-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-conversationmember-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="278a7-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="278a7-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-conversationmember-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="278a7-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="278a7-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-conversationmember-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="278a7-139">Java</span><span class="sxs-lookup"><span data-stu-id="278a7-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-conversationmember-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="278a7-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="278a7-140">Response</span></span>
<span data-ttu-id="278a7-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="278a7-141">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "name": "get_conversationmember",
  "@odata.type": "collection(microsoft.graph.aadUserConversationMember)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams('ee0f5ae2-8bc6-4ae5-8466-7daeebbfa062')/members",
    "@odata.count": 2,
    "value": [
        {
            "@odata.type": "#microsoft.graph.aadUserConversationMember",
            "id": "ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=",
            "roles": [],
            "displayName": "Adele Vance",
            "userId": "73761f06-2ac9-469c-9f10-279a8cc267f9",
            "email": "AdeleV@M365x987948.OnMicrosoft.com"
        },
        {
            "@odata.type": "#microsoft.graph.aadUserConversationMember",
            "id": "ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM1OThlZmNkNC1lNTQ5LTQwMmEtOTYwMi0wYjUwMjAxZmFlYmU=",
            "roles": [
                "owner"
            ],
            "displayName": "MOD Administrator",
            "userId": "598efcd4-e549-402a-9602-0b50201faebe",
            "email": "admin@M365x987948.OnMicrosoft.com"
        }
    ]
}
```
