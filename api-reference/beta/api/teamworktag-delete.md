---
title: Excluir teamworkTag
description: Exclui um objeto teamworkTag.
author: anniecolonna
localization_priority: Normal
ms.prod: teamwork
doc_type: apiPageType
ms.openlocfilehash: 3e23cd6e55122c81973e634cbc47ddaf88402c2d
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/22/2021
ms.locfileid: "53060669"
---
# <a name="delete-teamworktag"></a><span data-ttu-id="3b059-103">Excluir teamworkTag</span><span class="sxs-lookup"><span data-stu-id="3b059-103">Delete teamworkTag</span></span>
<span data-ttu-id="3b059-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3b059-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3b059-105">Exclua [um objeto tag.](../resources/teamworktag.md)</span><span class="sxs-lookup"><span data-stu-id="3b059-105">Delete a [tag](../resources/teamworktag.md) object.</span></span> 

## <a name="permissions"></a><span data-ttu-id="3b059-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="3b059-106">Permissions</span></span>
<span data-ttu-id="3b059-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3b059-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b059-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3b059-109">Permission type</span></span>|<span data-ttu-id="3b059-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3b059-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3b059-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3b059-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3b059-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3b059-112">Not supported.</span></span>|
|<span data-ttu-id="3b059-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3b059-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3b059-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3b059-114">Not supported.</span></span>|
|<span data-ttu-id="3b059-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3b059-115">Application</span></span>|<span data-ttu-id="3b059-116">TeamworkTag.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b059-116">TeamworkTag.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3b059-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3b059-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /teams/{team-Id}/tags/{teamworkTag-Id}
```

## <a name="request-headers"></a><span data-ttu-id="3b059-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3b059-118">Request headers</span></span>
|<span data-ttu-id="3b059-119">Nome</span><span class="sxs-lookup"><span data-stu-id="3b059-119">Name</span></span>|<span data-ttu-id="3b059-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="3b059-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="3b059-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="3b059-121">Authorization</span></span>|<span data-ttu-id="3b059-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3b059-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3b059-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3b059-124">Request body</span></span>
<span data-ttu-id="3b059-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3b059-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3b059-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b059-126">Response</span></span>

<span data-ttu-id="3b059-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="3b059-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="3b059-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="3b059-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3b059-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3b059-129">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_teamworktag"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/teams/53c53217-fe77-4383-bc5a-ed4937a1aecd/tags/MjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyM3ZDg4M2Q4Yi1hMTc5LTRkZDctOTNiMy1hOGQzZGUxYTIxMmUjI3RhY29VSjN2RGk==
```


### <a name="response"></a><span data-ttu-id="3b059-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b059-130">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

