---
title: Obter trabalho em equipeTagMember
description: Leia as propriedades e as relações de um objeto teamworkTagMember.
author: anniecolonna
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 8978cd5fe2ce6fc2ce806dc4093d50d86dc7c335
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/22/2021
ms.locfileid: "53060642"
---
# <a name="get-teamworktagmember"></a><span data-ttu-id="59059-103">Obter trabalho em equipeTagMember</span><span class="sxs-lookup"><span data-stu-id="59059-103">Get teamworkTagMember</span></span>
<span data-ttu-id="59059-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="59059-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="59059-105">Obter as propriedades e as relações de [um membro](../resources/teamworktagmember.md) de uma marca padrão em uma equipe.</span><span class="sxs-lookup"><span data-stu-id="59059-105">Get the properties and relationships of a [member](../resources/teamworktagmember.md) of a standard tag in a team.</span></span> 

## <a name="permissions"></a><span data-ttu-id="59059-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="59059-106">Permissions</span></span>
<span data-ttu-id="59059-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="59059-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59059-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="59059-109">Permission type</span></span>|<span data-ttu-id="59059-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="59059-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="59059-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="59059-111">Delegated (work or school account)</span></span>|<span data-ttu-id="59059-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="59059-112">Not supported.</span></span>|
|<span data-ttu-id="59059-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="59059-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="59059-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="59059-114">Not supported.</span></span>|
|<span data-ttu-id="59059-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="59059-115">Application</span></span>|<span data-ttu-id="59059-116">TeamworkTag.Read.All, TeamworkTag.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59059-116">TeamworkTag.Read.All, TeamworkTag.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="59059-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="59059-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /teams/{team-Id}/tags/{teamworkTag-Id}/members/{teamworkTagMember-Id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="59059-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="59059-118">Optional query parameters</span></span>
<span data-ttu-id="59059-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="59059-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="59059-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="59059-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="59059-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="59059-121">Request headers</span></span>
|<span data-ttu-id="59059-122">Nome</span><span class="sxs-lookup"><span data-stu-id="59059-122">Name</span></span>|<span data-ttu-id="59059-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="59059-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="59059-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="59059-124">Authorization</span></span>|<span data-ttu-id="59059-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="59059-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="59059-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="59059-127">Request body</span></span>
<span data-ttu-id="59059-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="59059-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="59059-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="59059-129">Response</span></span>

<span data-ttu-id="59059-130">Se tiver êxito, este método retornará um código de resposta e um `200 OK` objeto [teamworkTagMember](../resources/teamworktagmember.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="59059-130">If successful, this method returns a `200 OK` response code and a [teamworkTagMember](../resources/teamworktagmember.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="59059-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="59059-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="59059-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="59059-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_teamworktagmember"
}
-->
``` http
GET https://graph.microsoft.com/beta/teams/53c53217-fe77-4383-bc5a-ed4937a1aecd/tags/MjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyM3ZDg4M2Q4Yi1hMTc5LTRkZDctOTNiMy1hOGQzZGUxYTIxMmUjI3RhY29VSjN2RGk==/members/MjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyNlYjY1M2Y5Mi04MzczLTRkZTYtYmZlYy01YjRkMjE2YjZhZGUjI2QzYjJiM2ViLWM0N2YtNDViOS05NWYyLWIyZjJlZjYyMTVjZQ==
```


### <a name="response"></a><span data-ttu-id="59059-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="59059-133">Response</span></span>
><span data-ttu-id="59059-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="59059-134">**Note:** The response object shown here might be shortened for readability.</span></span>
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
