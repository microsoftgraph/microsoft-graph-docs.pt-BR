---
title: Obter teamworkTag
description: Leia as propriedades e as relações de um objeto teamworkTag.
author: anniecolonna
localization_priority: Normal
ms.prod: teamwork
doc_type: apiPageType
ms.openlocfilehash: 25ca36ae0d4f6a1fb6c4ffe14beb594c67fb316a
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53210248"
---
# <a name="get-teamworktag"></a><span data-ttu-id="61344-103">Obter teamworkTag</span><span class="sxs-lookup"><span data-stu-id="61344-103">Get teamworkTag</span></span>
<span data-ttu-id="61344-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="61344-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="61344-105">Leia as propriedades e as relações de um [objeto tag.](../resources/teamworktag.md)</span><span class="sxs-lookup"><span data-stu-id="61344-105">Read the properties and relationships of a [tag](../resources/teamworktag.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="61344-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="61344-106">Permissions</span></span>
<span data-ttu-id="61344-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="61344-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="61344-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="61344-109">Permission type</span></span>|<span data-ttu-id="61344-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="61344-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="61344-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="61344-111">Delegated (work or school account)</span></span>|<span data-ttu-id="61344-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="61344-112">Not supported.</span></span>|
|<span data-ttu-id="61344-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="61344-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="61344-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="61344-114">Not supported.</span></span>|
|<span data-ttu-id="61344-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="61344-115">Application</span></span>|<span data-ttu-id="61344-116">TeamworkTag.Read.All, TeamworkTag.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61344-116">TeamworkTag.Read.All, TeamworkTag.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="61344-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="61344-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /teams/{team-Id}/tags/{teamworkTag-Id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="61344-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="61344-118">Optional query parameters</span></span>
<span data-ttu-id="61344-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="61344-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="61344-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="61344-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="61344-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="61344-121">Request headers</span></span>
|<span data-ttu-id="61344-122">Nome</span><span class="sxs-lookup"><span data-stu-id="61344-122">Name</span></span>|<span data-ttu-id="61344-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="61344-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="61344-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="61344-124">Authorization</span></span>|<span data-ttu-id="61344-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="61344-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="61344-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="61344-127">Request body</span></span>
<span data-ttu-id="61344-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="61344-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="61344-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="61344-129">Response</span></span>

<span data-ttu-id="61344-130">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [teamworkTag](../resources/teamworktag.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="61344-130">If successful, this method returns a `200 OK` response code and a [teamworkTag](../resources/teamworktag.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="61344-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="61344-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="61344-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="61344-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="61344-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="61344-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_teamworktag"
}
-->
``` http
GET https://graph.microsoft.com/beta/teams/53c53217-fe77-4383-bc5a-ed4937a1aecd/tags/MjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyM3ZDg4M2Q4Yi1hMTc5LTRkZDctOTNiMy1hOGQzZGUxYTIxMmUjI3RhY29VSjN2RGk==
```
# <a name="c"></a>[<span data-ttu-id="61344-134">C#</span><span class="sxs-lookup"><span data-stu-id="61344-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-teamworktag-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="61344-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="61344-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-teamworktag-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="61344-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="61344-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-teamworktag-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="61344-137">Java</span><span class="sxs-lookup"><span data-stu-id="61344-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-teamworktag-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="61344-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="61344-138">Response</span></span>
><span data-ttu-id="61344-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="61344-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamworkTag"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.teamworkTag",
    "id": "MjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyM3ZDg4M2Q4Yi1hMTc5LTRkZDctOTNiMy1hOGQzZGUxYTIxMmUjI3RhY29VSjN2RGk==",
    "teamId": "53c53217-fe77-4383-bc5a-ed4937a1aecd",
    "displayName": "IT Admins",
    "description": "Team admins and IT support",
    "memberCount": "2",
    "tagType": "standard"
  }
}
```

