---
title: Criar teamworkTag
description: Crie um novo objeto teamworkTag.
author: anniecolonna
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: b379037f01b5d28c867de0083ec6f7a581f0ea80
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/22/2021
ms.locfileid: "53060645"
---
# <a name="create-teamworktag"></a><span data-ttu-id="d3e0a-103">Criar teamworkTag</span><span class="sxs-lookup"><span data-stu-id="d3e0a-103">Create teamworkTag</span></span>
<span data-ttu-id="d3e0a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3e0a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d3e0a-105">Crie uma [marca padrão](../resources/teamworktag.md) para membros na equipe.</span><span class="sxs-lookup"><span data-stu-id="d3e0a-105">Create a standard [tag](../resources/teamworktag.md) for members in the team.</span></span> 

## <a name="permissions"></a><span data-ttu-id="d3e0a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d3e0a-106">Permissions</span></span>
<span data-ttu-id="d3e0a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d3e0a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3e0a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d3e0a-109">Permission type</span></span>|<span data-ttu-id="d3e0a-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d3e0a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d3e0a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d3e0a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d3e0a-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d3e0a-112">Not supported.</span></span>|
|<span data-ttu-id="d3e0a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d3e0a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d3e0a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d3e0a-114">Not supported.</span></span>|
|<span data-ttu-id="d3e0a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d3e0a-115">Application</span></span>|<span data-ttu-id="d3e0a-116">TeamworkTag.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3e0a-116">TeamworkTag.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d3e0a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d3e0a-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /teams/{team-Id}/tags
```

## <a name="request-headers"></a><span data-ttu-id="d3e0a-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d3e0a-118">Request headers</span></span>
|<span data-ttu-id="d3e0a-119">Nome</span><span class="sxs-lookup"><span data-stu-id="d3e0a-119">Name</span></span>|<span data-ttu-id="d3e0a-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="d3e0a-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d3e0a-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="d3e0a-121">Authorization</span></span>|<span data-ttu-id="d3e0a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d3e0a-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="d3e0a-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d3e0a-124">Content-Type</span></span>|<span data-ttu-id="d3e0a-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d3e0a-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d3e0a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d3e0a-127">Request body</span></span>
<span data-ttu-id="d3e0a-128">No corpo da solicitação, fornece uma representação JSON do [objeto teamworkTag.](../resources/teamworktag.md)</span><span class="sxs-lookup"><span data-stu-id="d3e0a-128">In the request body, supply a JSON representation of the [teamworkTag](../resources/teamworktag.md) object.</span></span>

<span data-ttu-id="d3e0a-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o trabalho em [equipeTag](../resources/teamworktag.md).</span><span class="sxs-lookup"><span data-stu-id="d3e0a-129">The following table shows the properties that are required when you create the [teamworkTag](../resources/teamworktag.md).</span></span>

|<span data-ttu-id="d3e0a-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d3e0a-130">Property</span></span>|<span data-ttu-id="d3e0a-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d3e0a-131">Type</span></span>|<span data-ttu-id="d3e0a-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d3e0a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3e0a-133">displayName</span><span class="sxs-lookup"><span data-stu-id="d3e0a-133">displayName</span></span>|<span data-ttu-id="d3e0a-134">String</span><span class="sxs-lookup"><span data-stu-id="d3e0a-134">String</span></span>|<span data-ttu-id="d3e0a-135">Nome da marca.</span><span class="sxs-lookup"><span data-stu-id="d3e0a-135">Name of the tag.</span></span> <span data-ttu-id="d3e0a-136">O valor não pode ter mais de 40 caracteres.</span><span class="sxs-lookup"><span data-stu-id="d3e0a-136">The value cannot be more than 40 characters.</span></span>|
|<span data-ttu-id="d3e0a-137">membros</span><span class="sxs-lookup"><span data-stu-id="d3e0a-137">members</span></span>| <span data-ttu-id="d3e0a-138">[coleção teamworkTagMember](../resources/teamworktagmember.md)</span><span class="sxs-lookup"><span data-stu-id="d3e0a-138">[teamworkTagMember](../resources/teamworktagmember.md) collection</span></span> |<span data-ttu-id="d3e0a-139">Membros da equipe a adicionar à marca.</span><span class="sxs-lookup"><span data-stu-id="d3e0a-139">Members of the team to add to the tag.</span></span> <span data-ttu-id="d3e0a-140">De definir a propriedade do identificador de usuário de cada membro.</span><span class="sxs-lookup"><span data-stu-id="d3e0a-140">Set the user identifier property of each member.</span></span> <span data-ttu-id="d3e0a-141">A contagem de membros não deve ter mais de 25.</span><span class="sxs-lookup"><span data-stu-id="d3e0a-141">Members count should not be more than 25.</span></span>|



## <a name="response"></a><span data-ttu-id="d3e0a-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3e0a-142">Response</span></span>

<span data-ttu-id="d3e0a-143">Se tiver êxito, este método retornará um código `201 Created` de resposta e um objeto [teamworkTag](../resources/teamworktag.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d3e0a-143">If successful, this method returns a `201 Created` response code and a [teamworkTag](../resources/teamworktag.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d3e0a-144">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d3e0a-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d3e0a-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d3e0a-145">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_teamworktag_from"
}
-->
``` http
POST https://graph.microsoft.com/beta/teams/53c53217-fe77-4383-bc5a-ed4937a1aecd/tags
Content-Type: application/json

{
  "displayName": "Finance",
  "members":[
    {
        "userId":"92f6952f-61ca-4a94-8910-508a240bc167"
    },
    {
        "userId":"085d800c-b86b-4bfc-a857-9371ad1caf29"
    }
  ]
}
```


### <a name="response"></a><span data-ttu-id="d3e0a-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3e0a-146">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamworkTag"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.teamworkTag",
  "id": "MjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyM3ZDg4M2Q4Yi1hMTc5LTRkZDctOTNiMy1hOGQzZGUxYTIxMmUjI3RhY29VSjN2RGk==",
  "teamId": "53c53217-fe77-4383-bc5a-ed4937a1aecd",
  "displayName": "Financee",
  "memberCount": 2,
  "tagType": "standard"
}
```

