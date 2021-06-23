---
title: Listar teamworkTags
description: Obter uma lista dos objetos teamworkTag e suas propriedades.
author: anniecolonna
localization_priority: Normal
ms.prod: teamwork
doc_type: apiPageType
ms.openlocfilehash: 0a5e008e32565675982ec7d120be3d6d3bad98ed
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/22/2021
ms.locfileid: "53060647"
---
# <a name="list-teamworktags"></a><span data-ttu-id="d006c-103">Listar teamworkTags</span><span class="sxs-lookup"><span data-stu-id="d006c-103">List teamworkTags</span></span>
<span data-ttu-id="d006c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d006c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d006c-105">Obter uma lista dos [objetos tags](../resources/teamworktag.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="d006c-105">Get a list of the [tags](../resources/teamworktag.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="d006c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d006c-106">Permissions</span></span>
<span data-ttu-id="d006c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d006c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d006c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d006c-109">Permission type</span></span>|<span data-ttu-id="d006c-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d006c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d006c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d006c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d006c-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d006c-112">Not supported.</span></span>|
|<span data-ttu-id="d006c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d006c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d006c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d006c-114">Not supported.</span></span>|
|<span data-ttu-id="d006c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d006c-115">Application</span></span>|<span data-ttu-id="d006c-116">TeamworkTag.Read.All, TeamworkTag.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d006c-116">TeamworkTag.Read.All, TeamworkTag.ReadWrite.All</span></span>|

## <a name="relationships"></a><span data-ttu-id="d006c-117">Relações</span><span class="sxs-lookup"><span data-stu-id="d006c-117">Relationships</span></span>
|<span data-ttu-id="d006c-118">Relação</span><span class="sxs-lookup"><span data-stu-id="d006c-118">Relationship</span></span>|<span data-ttu-id="d006c-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="d006c-119">Type</span></span>|<span data-ttu-id="d006c-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="d006c-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d006c-121">membros</span><span class="sxs-lookup"><span data-stu-id="d006c-121">members</span></span>|<span data-ttu-id="d006c-122">[coleção teamworkTag](../resources/teamworktag.md)</span><span class="sxs-lookup"><span data-stu-id="d006c-122">[teamworkTag](../resources/teamworktag.md) collection</span></span>|<span data-ttu-id="d006c-123">Marcas atribuídas a uma equipe.</span><span class="sxs-lookup"><span data-stu-id="d006c-123">Tags assigned to a team.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d006c-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d006c-124">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /teams/{team-Id}/tags
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d006c-125">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d006c-125">Optional query parameters</span></span>
<span data-ttu-id="d006c-126">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d006c-126">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="d006c-127">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="d006c-127">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="d006c-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d006c-128">Request headers</span></span>
|<span data-ttu-id="d006c-129">Nome</span><span class="sxs-lookup"><span data-stu-id="d006c-129">Name</span></span>|<span data-ttu-id="d006c-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="d006c-130">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d006c-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="d006c-131">Authorization</span></span>|<span data-ttu-id="d006c-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d006c-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d006c-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d006c-134">Request body</span></span>
<span data-ttu-id="d006c-135">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d006c-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d006c-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="d006c-136">Response</span></span>

<span data-ttu-id="d006c-137">Se tiver êxito, este método retornará um código `200 OK` de resposta e uma coleção de objetos [teamworkTag](../resources/teamworktag.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d006c-137">If successful, this method returns a `200 OK` response code and a collection of [teamworkTag](../resources/teamworktag.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d006c-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d006c-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d006c-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d006c-139">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_teamworktag"
}
-->
``` http
GET https://graph.microsoft.com/beta/teams/53c53217-fe77-4383-bc5a-ed4937a1aecd/tags
```


### <a name="response"></a><span data-ttu-id="d006c-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="d006c-140">Response</span></span>
><span data-ttu-id="d006c-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d006c-141">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.teamworkTag)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
        "@odata.type": "#microsoft.graph.teamworkTag",
        "id": "MjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyM3ZDg4M2Q4Yi1hMTc5LTRkZDctOTNiMy1hOGQzZGUxYTIxMmUjI3RhY29VSjN2RGk==",
        "teamId": "53c53217-fe77-4383-bc5a-ed4937a1aecd",
        "displayName": "Finance",
        "description": "Finance Team for Mach 8 Project",
        "memberCount": 2,
        "tagType": "standard"
    },
    {
        "@odata.type": "#microsoft.graph.teamworkTag",
        "id": "MjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyNlYjY1M2Y5Mi04MzczLTRkZTYtYmZlYy01YjRkMjE2YjZhZGUjIzk3ZjYyMzQ0LTU3ZGMtNDA5Yy04OGFkLWM0YWYxNDE1OGZmNQ==",
        "teamId": "53c53217-fe77-4383-bc5a-ed4937a1aecd",
        "displayName": "Legal",
        "description": "Legal experts, ask us your legal questions",
        "memberCount": 4,
        "tagType": "standard"
    }
  ]
}
```

