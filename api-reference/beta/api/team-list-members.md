---
title: Listar membros
description: Obtenha o conversationMembers de uma equipe.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 9adfa391634164af0818bd81b2cc33d9969a79df
ms.sourcegitcommit: 67433748b69541727185fc1f32ed356718bf6ff1
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2020
ms.locfileid: "45050988"
---
# <a name="list-members"></a><span data-ttu-id="f8bc0-103">Listar membros</span><span class="sxs-lookup"><span data-stu-id="f8bc0-103">List members</span></span>
<span data-ttu-id="f8bc0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f8bc0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f8bc0-105">Obtenha o [conversationMember](../resources/conversationmember.md) de uma [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="f8bc0-105">Get the [conversationMember](../resources/conversationmember.md) of a [team](../resources/team.md).</span></span>

><span data-ttu-id="f8bc0-106">Observação: essa API atualmente não oferece suporte à paginação, portanto, se houver muitos membros para caber em uma solicitação, você não receberá todos os membros.</span><span class="sxs-lookup"><span data-stu-id="f8bc0-106">Note: This API currently does not support pagination, so if there's too many members to fit into one request, you won't get all the members.</span></span>

## <a name="permissions"></a><span data-ttu-id="f8bc0-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="f8bc0-107">Permissions</span></span>
<span data-ttu-id="f8bc0-108">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="f8bc0-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="f8bc0-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f8bc0-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f8bc0-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f8bc0-110">Permission type</span></span>|<span data-ttu-id="f8bc0-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f8bc0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f8bc0-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f8bc0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f8bc0-113">TeamMember. Read. All, TeamMember. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="f8bc0-113">TeamMember.Read.All, TeamMember.ReadWrite.All</span></span>|
|<span data-ttu-id="f8bc0-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f8bc0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f8bc0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f8bc0-115">Not supported.</span></span>    |
|<span data-ttu-id="f8bc0-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f8bc0-116">Application</span></span>|<span data-ttu-id="f8bc0-117">TeamMember. Read. All, TeamMember. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="f8bc0-117">TeamMember.Read.All, TeamMember.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f8bc0-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f8bc0-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /teams/{teamsId}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f8bc0-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f8bc0-119">Optional query parameters</span></span>
<span data-ttu-id="f8bc0-120">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f8bc0-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="f8bc0-121">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="f8bc0-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="f8bc0-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f8bc0-122">Request headers</span></span>
|<span data-ttu-id="f8bc0-123">Nome</span><span class="sxs-lookup"><span data-stu-id="f8bc0-123">Name</span></span>|<span data-ttu-id="f8bc0-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="f8bc0-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f8bc0-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="f8bc0-125">Authorization</span></span>|<span data-ttu-id="f8bc0-126">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="f8bc0-126">Bearer {token}.</span></span> <span data-ttu-id="f8bc0-127">Required.</span><span class="sxs-lookup"><span data-stu-id="f8bc0-127">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f8bc0-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f8bc0-128">Request body</span></span>
<span data-ttu-id="f8bc0-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f8bc0-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f8bc0-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="f8bc0-130">Response</span></span>

<span data-ttu-id="f8bc0-131">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [conversationMember](../resources/conversationmember.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f8bc0-131">If successful, this method returns a `200 OK` response code and a collection of [conversationMember](../resources/conversationmember.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f8bc0-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f8bc0-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f8bc0-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f8bc0-133">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_conversationmember"
}
-->
``` http
GET https://graph.microsoft.com/beta/teams/{teamsId}/members
```


### <a name="response"></a><span data-ttu-id="f8bc0-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="f8bc0-134">Response</span></span>
<span data-ttu-id="f8bc0-135">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="f8bc0-135">**Note:** The response object shown here might be shortened for readability.</span></span>
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
