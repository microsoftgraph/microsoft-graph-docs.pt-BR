---
title: Obter teamworkTag
description: Leia as propriedades e as relações de um objeto teamworkTag.
author: anniecolonna
localization_priority: Normal
ms.prod: teamwork
doc_type: apiPageType
ms.openlocfilehash: aa99a204fac9dbc2417d0e30d548638e0b63ebd6
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/22/2021
ms.locfileid: "53060648"
---
# <a name="get-teamworktag"></a><span data-ttu-id="b4060-103">Obter teamworkTag</span><span class="sxs-lookup"><span data-stu-id="b4060-103">Get teamworkTag</span></span>
<span data-ttu-id="b4060-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b4060-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b4060-105">Leia as propriedades e as relações de um [objeto tag.](../resources/teamworktag.md)</span><span class="sxs-lookup"><span data-stu-id="b4060-105">Read the properties and relationships of a [tag](../resources/teamworktag.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b4060-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b4060-106">Permissions</span></span>
<span data-ttu-id="b4060-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b4060-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b4060-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b4060-109">Permission type</span></span>|<span data-ttu-id="b4060-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b4060-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b4060-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b4060-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b4060-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b4060-112">Not supported.</span></span>|
|<span data-ttu-id="b4060-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b4060-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b4060-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b4060-114">Not supported.</span></span>|
|<span data-ttu-id="b4060-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b4060-115">Application</span></span>|<span data-ttu-id="b4060-116">TeamworkTag.Read.All, TeamworkTag.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4060-116">TeamworkTag.Read.All, TeamworkTag.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b4060-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b4060-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /teams/{team-Id}/tags/{teamworkTag-Id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b4060-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b4060-118">Optional query parameters</span></span>
<span data-ttu-id="b4060-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b4060-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="b4060-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="b4060-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="b4060-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b4060-121">Request headers</span></span>
|<span data-ttu-id="b4060-122">Nome</span><span class="sxs-lookup"><span data-stu-id="b4060-122">Name</span></span>|<span data-ttu-id="b4060-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="b4060-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b4060-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="b4060-124">Authorization</span></span>|<span data-ttu-id="b4060-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b4060-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b4060-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b4060-127">Request body</span></span>
<span data-ttu-id="b4060-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b4060-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b4060-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="b4060-129">Response</span></span>

<span data-ttu-id="b4060-130">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [teamworkTag](../resources/teamworktag.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b4060-130">If successful, this method returns a `200 OK` response code and a [teamworkTag](../resources/teamworktag.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b4060-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b4060-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b4060-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b4060-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_teamworktag"
}
-->
``` http
GET https://graph.microsoft.com/beta/teams/53c53217-fe77-4383-bc5a-ed4937a1aecd/tags/MjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyM3ZDg4M2Q4Yi1hMTc5LTRkZDctOTNiMy1hOGQzZGUxYTIxMmUjI3RhY29VSjN2RGk==
```


### <a name="response"></a><span data-ttu-id="b4060-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="b4060-133">Response</span></span>
><span data-ttu-id="b4060-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b4060-134">**Note:** The response object shown here might be shortened for readability.</span></span>
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

