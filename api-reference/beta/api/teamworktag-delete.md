---
title: Excluir teamworkTag
description: Exclui um objeto teamworkTag.
author: anniecolonna
localization_priority: Normal
ms.prod: teamwork
doc_type: apiPageType
ms.openlocfilehash: 169879fbc3bcd121f5edf270d90f4666a15a93ef
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53210210"
---
# <a name="delete-teamworktag"></a><span data-ttu-id="7be2f-103">Excluir teamworkTag</span><span class="sxs-lookup"><span data-stu-id="7be2f-103">Delete teamworkTag</span></span>
<span data-ttu-id="7be2f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7be2f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7be2f-105">Exclua [um objeto tag.](../resources/teamworktag.md)</span><span class="sxs-lookup"><span data-stu-id="7be2f-105">Delete a [tag](../resources/teamworktag.md) object.</span></span> 

## <a name="permissions"></a><span data-ttu-id="7be2f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="7be2f-106">Permissions</span></span>
<span data-ttu-id="7be2f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7be2f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7be2f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7be2f-109">Permission type</span></span>|<span data-ttu-id="7be2f-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7be2f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7be2f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7be2f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7be2f-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7be2f-112">Not supported.</span></span>|
|<span data-ttu-id="7be2f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7be2f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7be2f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7be2f-114">Not supported.</span></span>|
|<span data-ttu-id="7be2f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7be2f-115">Application</span></span>|<span data-ttu-id="7be2f-116">TeamworkTag.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7be2f-116">TeamworkTag.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7be2f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7be2f-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /teams/{team-Id}/tags/{teamworkTag-Id}
```

## <a name="request-headers"></a><span data-ttu-id="7be2f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7be2f-118">Request headers</span></span>
|<span data-ttu-id="7be2f-119">Nome</span><span class="sxs-lookup"><span data-stu-id="7be2f-119">Name</span></span>|<span data-ttu-id="7be2f-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="7be2f-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="7be2f-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="7be2f-121">Authorization</span></span>|<span data-ttu-id="7be2f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7be2f-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7be2f-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7be2f-124">Request body</span></span>
<span data-ttu-id="7be2f-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7be2f-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7be2f-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="7be2f-126">Response</span></span>

<span data-ttu-id="7be2f-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="7be2f-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="7be2f-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="7be2f-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7be2f-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7be2f-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="7be2f-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="7be2f-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_teamworktag"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/teams/53c53217-fe77-4383-bc5a-ed4937a1aecd/tags/MjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyM3ZDg4M2Q4Yi1hMTc5LTRkZDctOTNiMy1hOGQzZGUxYTIxMmUjI3RhY29VSjN2RGk==
```
# <a name="c"></a>[<span data-ttu-id="7be2f-131">C#</span><span class="sxs-lookup"><span data-stu-id="7be2f-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-teamworktag-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7be2f-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7be2f-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-teamworktag-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7be2f-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7be2f-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-teamworktag-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7be2f-134">Java</span><span class="sxs-lookup"><span data-stu-id="7be2f-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-teamworktag-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="7be2f-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="7be2f-135">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

