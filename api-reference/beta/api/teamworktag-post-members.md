---
title: Criar trabalho em equipeTagMember
description: Crie um novo objeto teamworkTagMember.
author: anniecolonna
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 28ae8ae4749e1ecca4f5e370858e88de45d2faf4
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/22/2021
ms.locfileid: "53060646"
---
# <a name="create-teamworktagmember"></a><span data-ttu-id="a04d9-103">Criar trabalho em equipeTagMember</span><span class="sxs-lookup"><span data-stu-id="a04d9-103">Create teamworkTagMember</span></span>
<span data-ttu-id="a04d9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a04d9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a04d9-105">Crie um novo [objeto teamworkTagMember](../resources/teamworktagmember.md) em uma equipe.</span><span class="sxs-lookup"><span data-stu-id="a04d9-105">Create a new [teamworkTagMember](../resources/teamworktagmember.md) object in a team.</span></span>

## <a name="permissions"></a><span data-ttu-id="a04d9-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a04d9-106">Permissions</span></span>
<span data-ttu-id="a04d9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a04d9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a04d9-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a04d9-109">Permission type</span></span>|<span data-ttu-id="a04d9-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a04d9-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a04d9-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a04d9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a04d9-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a04d9-112">Not supported.</span></span>|
|<span data-ttu-id="a04d9-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a04d9-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a04d9-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a04d9-114">Not supported.</span></span>|
|<span data-ttu-id="a04d9-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a04d9-115">Application</span></span>|<span data-ttu-id="a04d9-116">TeamworkTag.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a04d9-116">TeamworkTag.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a04d9-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a04d9-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /teams/{team-Id}/tags/{teamworkTag-Id}/members
```

## <a name="request-headers"></a><span data-ttu-id="a04d9-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a04d9-118">Request headers</span></span>
|<span data-ttu-id="a04d9-119">Nome</span><span class="sxs-lookup"><span data-stu-id="a04d9-119">Name</span></span>|<span data-ttu-id="a04d9-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="a04d9-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a04d9-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="a04d9-121">Authorization</span></span>|<span data-ttu-id="a04d9-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a04d9-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="a04d9-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a04d9-124">Content-Type</span></span>|<span data-ttu-id="a04d9-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a04d9-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a04d9-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a04d9-127">Request body</span></span>
<span data-ttu-id="a04d9-128">No corpo da solicitação, fornece uma representação JSON do [objeto teamworkTagMember.](../resources/teamworktagmember.md)</span><span class="sxs-lookup"><span data-stu-id="a04d9-128">In the request body, supply a JSON representation of the [teamworkTagMember](../resources/teamworktagmember.md) object.</span></span>

<span data-ttu-id="a04d9-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o trabalho em [equipeTagMember](../resources/teamworktagmember.md).</span><span class="sxs-lookup"><span data-stu-id="a04d9-129">The following table shows the properties that are required when you create the [teamworkTagMember](../resources/teamworktagmember.md).</span></span>

|<span data-ttu-id="a04d9-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a04d9-130">Property</span></span>|<span data-ttu-id="a04d9-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a04d9-131">Type</span></span>|<span data-ttu-id="a04d9-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a04d9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a04d9-133">userId</span><span class="sxs-lookup"><span data-stu-id="a04d9-133">userId</span></span>|<span data-ttu-id="a04d9-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a04d9-134">String</span></span>|<span data-ttu-id="a04d9-135">Identificador de usuário do membro da equipe.</span><span class="sxs-lookup"><span data-stu-id="a04d9-135">User identifier of the member of the team.</span></span>|



## <a name="response"></a><span data-ttu-id="a04d9-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="a04d9-136">Response</span></span>

<span data-ttu-id="a04d9-137">Se tiver êxito, este método retornará um código de resposta e um `201 Created` objeto [teamworkTagMember](../resources/teamworktagmember.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a04d9-137">If successful, this method returns a `201 Created` response code and a [teamworkTagMember](../resources/teamworktagmember.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a04d9-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a04d9-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a04d9-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a04d9-139">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "create_teamworktagmember_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/teams/53c53217-fe77-4383-bc5a-ed4937a1aecd/tags/MjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyM3ZDg4M2Q4Yi1hMTc5LTRkZDctOTNiMy1hOGQzZGUxYTIxMmUjI3RhY29VSjN2RGk==/members
Content-Type: application/json
Content-length: 144

{
    "userId":"97f62344-57dc-409c-88ad-c4af14158ff5"
}
```


### <a name="response"></a><span data-ttu-id="a04d9-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="a04d9-140">Response</span></span>
><span data-ttu-id="a04d9-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a04d9-141">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamworkTagMember"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.type": "#microsoft.graph.teamworkTagMember",
    "id": "MjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyNlYjY1M2Y5Mi04MzczLTRkZTYtYmZlYy01YjRkMjE2YjZhZGUjI2QzYjJiM2ViLWM0N2YtNDViOS05NWYyLWIyZjJlZjYyMTVjZQ==",
    "displayName": "Megan Bowen",
    "tenantId": "18be64a9-c73a-4862-bccc-76c31ef09b9d",
    "userId": "92f6952f-61ca-4a94-8910-508a240bc167"
}
```

