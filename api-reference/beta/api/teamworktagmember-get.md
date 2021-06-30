---
title: Obter trabalho em equipeTagMember
description: Leia as propriedades e as relações de um objeto teamworkTagMember.
author: anniecolonna
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 91d9fb93306affa987faf73032ba182ef2b1689e
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53209951"
---
# <a name="get-teamworktagmember"></a><span data-ttu-id="56c6e-103">Obter trabalho em equipeTagMember</span><span class="sxs-lookup"><span data-stu-id="56c6e-103">Get teamworkTagMember</span></span>
<span data-ttu-id="56c6e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="56c6e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="56c6e-105">Obter as propriedades e as relações de [um membro](../resources/teamworktagmember.md) de uma marca padrão em uma equipe.</span><span class="sxs-lookup"><span data-stu-id="56c6e-105">Get the properties and relationships of a [member](../resources/teamworktagmember.md) of a standard tag in a team.</span></span> 

## <a name="permissions"></a><span data-ttu-id="56c6e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="56c6e-106">Permissions</span></span>
<span data-ttu-id="56c6e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="56c6e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="56c6e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="56c6e-109">Permission type</span></span>|<span data-ttu-id="56c6e-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="56c6e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="56c6e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="56c6e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="56c6e-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="56c6e-112">Not supported.</span></span>|
|<span data-ttu-id="56c6e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="56c6e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="56c6e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="56c6e-114">Not supported.</span></span>|
|<span data-ttu-id="56c6e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="56c6e-115">Application</span></span>|<span data-ttu-id="56c6e-116">TeamworkTag.Read.All, TeamworkTag.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56c6e-116">TeamworkTag.Read.All, TeamworkTag.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="56c6e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="56c6e-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /teams/{team-Id}/tags/{teamworkTag-Id}/members/{teamworkTagMember-Id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="56c6e-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="56c6e-118">Optional query parameters</span></span>
<span data-ttu-id="56c6e-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="56c6e-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="56c6e-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="56c6e-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="56c6e-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="56c6e-121">Request headers</span></span>
|<span data-ttu-id="56c6e-122">Nome</span><span class="sxs-lookup"><span data-stu-id="56c6e-122">Name</span></span>|<span data-ttu-id="56c6e-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="56c6e-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="56c6e-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="56c6e-124">Authorization</span></span>|<span data-ttu-id="56c6e-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="56c6e-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="56c6e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="56c6e-127">Request body</span></span>
<span data-ttu-id="56c6e-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="56c6e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="56c6e-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="56c6e-129">Response</span></span>

<span data-ttu-id="56c6e-130">Se tiver êxito, este método retornará um código de resposta e um `200 OK` objeto [teamworkTagMember](../resources/teamworktagmember.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="56c6e-130">If successful, this method returns a `200 OK` response code and a [teamworkTagMember](../resources/teamworktagmember.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="56c6e-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="56c6e-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="56c6e-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="56c6e-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="56c6e-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="56c6e-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_teamworktagmember"
}
-->
``` http
GET https://graph.microsoft.com/beta/teams/53c53217-fe77-4383-bc5a-ed4937a1aecd/tags/MjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyM3ZDg4M2Q4Yi1hMTc5LTRkZDctOTNiMy1hOGQzZGUxYTIxMmUjI3RhY29VSjN2RGk==/members/MjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyNlYjY1M2Y5Mi04MzczLTRkZTYtYmZlYy01YjRkMjE2YjZhZGUjI2QzYjJiM2ViLWM0N2YtNDViOS05NWYyLWIyZjJlZjYyMTVjZQ==
```
# <a name="c"></a>[<span data-ttu-id="56c6e-134">C#</span><span class="sxs-lookup"><span data-stu-id="56c6e-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-teamworktagmember-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="56c6e-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="56c6e-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-teamworktagmember-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="56c6e-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="56c6e-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-teamworktagmember-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="56c6e-137">Java</span><span class="sxs-lookup"><span data-stu-id="56c6e-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-teamworktagmember-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="56c6e-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="56c6e-138">Response</span></span>
><span data-ttu-id="56c6e-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="56c6e-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamworkTagMember"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.teamworkTagMember",
    "id": "MjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyNlYjY1M2Y5Mi04MzczLTRkZTYtYmZlYy01YjRkMjE2YjZhZGUjI2QzYjJiM2ViLWM0N2YtNDViOS05NWYyLWIyZjJlZjYyMTVjZQ==",
    "displayName": "Alex Wilbur",
    "tenantId": "18be64a9-c73a-4862-bccc-76c31ef09b9d",
    "userId": "92f6952f-61ca-4a94-8910-508a240bc167"
  }
}
```
