---
title: Listar membros
description: Obtenha o conversationMembers de uma equipe.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 2b9840ba7d543a01a8ed458489cf91c257c9f71f
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/14/2020
ms.locfileid: "45124104"
---
# <a name="list-members"></a><span data-ttu-id="45786-103">Listar membros</span><span class="sxs-lookup"><span data-stu-id="45786-103">List members</span></span>
<span data-ttu-id="45786-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="45786-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="45786-105">Obtenha o [conversationMember](../resources/conversationmember.md) de uma [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="45786-105">Get the [conversationMember](../resources/conversationmember.md) of a [team](../resources/team.md).</span></span>

><span data-ttu-id="45786-106">Observação: atualmente, esta API não é compatível com a paginação, portanto, se houver muitos membros para se ajustarem a uma solicitação, você não terá todos os membros.</span><span class="sxs-lookup"><span data-stu-id="45786-106">Note: This API currently does not support pagination, so if there's too many members to fit into one request, you won't get all the members.</span></span>

## <a name="permissions"></a><span data-ttu-id="45786-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="45786-107">Permissions</span></span>
<span data-ttu-id="45786-108">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="45786-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="45786-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="45786-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45786-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="45786-110">Permission type</span></span>|<span data-ttu-id="45786-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="45786-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="45786-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="45786-112">Delegated (work or school account)</span></span>|<span data-ttu-id="45786-113">TeamMember.Read.All, TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45786-113">TeamMember.Read.All, TeamMember.ReadWrite.All</span></span>|
|<span data-ttu-id="45786-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="45786-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="45786-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="45786-115">Not supported.</span></span>    |
|<span data-ttu-id="45786-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="45786-116">Application</span></span>|<span data-ttu-id="45786-117">TeamMember.Read.All, TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45786-117">TeamMember.Read.All, TeamMember.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="45786-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="45786-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /teams/{teamsId}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="45786-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="45786-119">Optional query parameters</span></span>
<span data-ttu-id="45786-120">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="45786-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="45786-121">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="45786-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="45786-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="45786-122">Request headers</span></span>
|<span data-ttu-id="45786-123">Nome</span><span class="sxs-lookup"><span data-stu-id="45786-123">Name</span></span>|<span data-ttu-id="45786-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="45786-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="45786-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="45786-125">Authorization</span></span>|<span data-ttu-id="45786-126">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="45786-126">Bearer {token}.</span></span> <span data-ttu-id="45786-127">Required.</span><span class="sxs-lookup"><span data-stu-id="45786-127">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="45786-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="45786-128">Request body</span></span>
<span data-ttu-id="45786-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="45786-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="45786-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="45786-130">Response</span></span>

<span data-ttu-id="45786-131">Se bem sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [conversationMember](../resources/conversationmember.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="45786-131">If successful, this method returns a `200 OK` response code and a collection of [conversationMember](../resources/conversationmember.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="45786-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="45786-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="45786-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="45786-133">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="45786-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="45786-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_conversationmember"
}
-->
``` http
GET https://graph.microsoft.com/beta/teams/{teamsId}/members
```
# <a name="c"></a>[<span data-ttu-id="45786-135">C#</span><span class="sxs-lookup"><span data-stu-id="45786-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-conversationmember-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="45786-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="45786-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-conversationmember-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="45786-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="45786-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-conversationmember-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="45786-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="45786-138">Response</span></span>
<span data-ttu-id="45786-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="45786-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('ee0f5ae2-8bc6-4ae5-8466-7daeebbfa062')/members",
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
