---
title: Listar membros
description: Obtenha o conversationMembers de uma equipe.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 214cd5fa426a72a6917431ce7a77287ead915858
ms.sourcegitcommit: 2050639c9e9a6b2dab9ce53d6a9fc87e98789b50
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/08/2020
ms.locfileid: "45081024"
---
# <a name="list-members"></a><span data-ttu-id="081d7-103">Listar membros</span><span class="sxs-lookup"><span data-stu-id="081d7-103">List members</span></span>
<span data-ttu-id="081d7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="081d7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="081d7-105">Obtenha o [conversationMember](../resources/conversationmember.md) de uma [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="081d7-105">Get the [conversationMember](../resources/conversationmember.md) of a [team](../resources/team.md).</span></span>

><span data-ttu-id="081d7-106">Observação: essa API atualmente não oferece suporte à paginação, portanto, se houver muitos membros para caber em uma solicitação, você não receberá todos os membros.</span><span class="sxs-lookup"><span data-stu-id="081d7-106">Note: This API currently does not support pagination, so if there's too many members to fit into one request, you won't get all the members.</span></span>

## <a name="permissions"></a><span data-ttu-id="081d7-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="081d7-107">Permissions</span></span>
<span data-ttu-id="081d7-108">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="081d7-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="081d7-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="081d7-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="081d7-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="081d7-110">Permission type</span></span>|<span data-ttu-id="081d7-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="081d7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="081d7-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="081d7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="081d7-113">TeamMember. Read. All, TeamMember. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="081d7-113">TeamMember.Read.All, TeamMember.ReadWrite.All</span></span>|
|<span data-ttu-id="081d7-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="081d7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="081d7-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="081d7-115">Not supported.</span></span>    |
|<span data-ttu-id="081d7-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="081d7-116">Application</span></span>|<span data-ttu-id="081d7-117">TeamMember. Read. All, TeamMember. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="081d7-117">TeamMember.Read.All, TeamMember.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="081d7-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="081d7-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /teams/{teamsId}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="081d7-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="081d7-119">Optional query parameters</span></span>
<span data-ttu-id="081d7-120">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="081d7-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="081d7-121">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="081d7-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="081d7-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="081d7-122">Request headers</span></span>
|<span data-ttu-id="081d7-123">Nome</span><span class="sxs-lookup"><span data-stu-id="081d7-123">Name</span></span>|<span data-ttu-id="081d7-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="081d7-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="081d7-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="081d7-125">Authorization</span></span>|<span data-ttu-id="081d7-126">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="081d7-126">Bearer {token}.</span></span> <span data-ttu-id="081d7-127">Required.</span><span class="sxs-lookup"><span data-stu-id="081d7-127">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="081d7-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="081d7-128">Request body</span></span>
<span data-ttu-id="081d7-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="081d7-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="081d7-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="081d7-130">Response</span></span>

<span data-ttu-id="081d7-131">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [conversationMember](../resources/conversationmember.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="081d7-131">If successful, this method returns a `200 OK` response code and a collection of [conversationMember](../resources/conversationmember.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="081d7-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="081d7-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="081d7-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="081d7-133">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="081d7-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="081d7-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_conversationmember"
}
-->
``` http
GET https://graph.microsoft.com/beta/teams/{teamsId}/members
```
# <a name="c"></a>[<span data-ttu-id="081d7-135">C#</span><span class="sxs-lookup"><span data-stu-id="081d7-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-conversationmember-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="081d7-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="081d7-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-conversationmember-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="081d7-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="081d7-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-conversationmember-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="081d7-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="081d7-138">Response</span></span>
<span data-ttu-id="081d7-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="081d7-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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
