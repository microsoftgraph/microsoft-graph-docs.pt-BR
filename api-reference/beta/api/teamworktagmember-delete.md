---
title: Excluir o trabalho em equipeTagMember
description: Excluir um objeto teamworkTagMember.
author: anniecolonna
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: ab64e7053757fed77a086bbdbde4c408813b1879
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/22/2021
ms.locfileid: "53060643"
---
# <a name="delete-teamworktagmember"></a><span data-ttu-id="a7ef3-103">Excluir o trabalho em equipeTagMember</span><span class="sxs-lookup"><span data-stu-id="a7ef3-103">Delete teamworkTagMember</span></span>
<span data-ttu-id="a7ef3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a7ef3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a7ef3-105">[Exclua um membro](../resources/teamworktagmember.md) de uma marca padrão na equipe.</span><span class="sxs-lookup"><span data-stu-id="a7ef3-105">Delete a [member](../resources/teamworktagmember.md) from a standard tag in the team.</span></span> 

## <a name="permissions"></a><span data-ttu-id="a7ef3-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a7ef3-106">Permissions</span></span>
<span data-ttu-id="a7ef3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a7ef3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a7ef3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a7ef3-109">Permission type</span></span>|<span data-ttu-id="a7ef3-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a7ef3-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a7ef3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a7ef3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a7ef3-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a7ef3-112">Not supported.</span></span>|
|<span data-ttu-id="a7ef3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a7ef3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a7ef3-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a7ef3-114">Not supported.</span></span>|
|<span data-ttu-id="a7ef3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a7ef3-115">Application</span></span>|<span data-ttu-id="a7ef3-116">TeamworkTag.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a7ef3-116">TeamworkTag.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a7ef3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a7ef3-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /teams/{team-Id}/tags/{teamworkTag-Id}/members/{teamworkTagMember-Id}
```

## <a name="request-headers"></a><span data-ttu-id="a7ef3-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a7ef3-118">Request headers</span></span>
|<span data-ttu-id="a7ef3-119">Nome</span><span class="sxs-lookup"><span data-stu-id="a7ef3-119">Name</span></span>|<span data-ttu-id="a7ef3-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="a7ef3-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a7ef3-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="a7ef3-121">Authorization</span></span>|<span data-ttu-id="a7ef3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a7ef3-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a7ef3-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a7ef3-124">Request body</span></span>
<span data-ttu-id="a7ef3-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a7ef3-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a7ef3-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="a7ef3-126">Response</span></span>

<span data-ttu-id="a7ef3-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a7ef3-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="a7ef3-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a7ef3-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a7ef3-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a7ef3-129">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_teamworktagmember"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/teams/53c53217-fe77-4383-bc5a-ed4937a1aecd/tags/MjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyM3ZDg4M2Q4Yi1hMTc5LTRkZDctOTNiMy1hOGQzZGUxYTIxMmUjI3RhY29VSjN2RGk==/members/MjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyNlYjY1M2Y5Mi04MzczLTRkZTYtYmZlYy01YjRkMjE2YjZhZGUjI2QzYjJiM2ViLWM0N2YtNDViOS05NWYyLWIyZjJlZjYyMTVjZQ==
```


### <a name="response"></a><span data-ttu-id="a7ef3-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="a7ef3-130">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
