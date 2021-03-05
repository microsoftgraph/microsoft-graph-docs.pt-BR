---
title: 'groupLifecyclePolicy: removeGroup'
description: Remove um grupo de uma política de ciclo de vida.
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: b0ee54109fe69938ad2f9169e3caf35232c9f5d5
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50474474"
---
# <a name="grouplifecyclepolicy-removegroup"></a><span data-ttu-id="11f79-103">groupLifecyclePolicy: removeGroup</span><span class="sxs-lookup"><span data-stu-id="11f79-103">groupLifecyclePolicy: removeGroup</span></span>

<span data-ttu-id="11f79-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="11f79-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="11f79-105">Remove um grupo de uma política de ciclo de vida.</span><span class="sxs-lookup"><span data-stu-id="11f79-105">Removes a group from a lifecycle policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="11f79-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="11f79-106">Permissions</span></span>

<span data-ttu-id="11f79-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="11f79-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="11f79-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="11f79-109">Permission type</span></span>      | <span data-ttu-id="11f79-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="11f79-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="11f79-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="11f79-111">Delegated (work or school account)</span></span> | <span data-ttu-id="11f79-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11f79-112">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="11f79-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="11f79-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="11f79-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="11f79-114">Not supported.</span></span>    |
|<span data-ttu-id="11f79-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="11f79-115">Application</span></span> | <span data-ttu-id="11f79-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11f79-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="11f79-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="11f79-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies/{id}/removeGroup
```

## <a name="request-headers"></a><span data-ttu-id="11f79-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="11f79-118">Request headers</span></span>

| <span data-ttu-id="11f79-119">Nome</span><span class="sxs-lookup"><span data-stu-id="11f79-119">Name</span></span> | <span data-ttu-id="11f79-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="11f79-120">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="11f79-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="11f79-121">Authorization</span></span> | <span data-ttu-id="11f79-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="11f79-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="11f79-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="11f79-124">Content-Type</span></span>  | <span data-ttu-id="11f79-125">application/json</span><span class="sxs-lookup"><span data-stu-id="11f79-125">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="11f79-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="11f79-126">Request body</span></span>
<span data-ttu-id="11f79-127">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="11f79-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="11f79-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="11f79-128">Parameter</span></span> | <span data-ttu-id="11f79-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="11f79-129">Type</span></span> | <span data-ttu-id="11f79-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="11f79-130">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="11f79-131">groupId</span><span class="sxs-lookup"><span data-stu-id="11f79-131">groupId</span></span>|<span data-ttu-id="11f79-132">Guid</span><span class="sxs-lookup"><span data-stu-id="11f79-132">Guid</span></span>| <span data-ttu-id="11f79-133">A ID do grupo que será removido da política.</span><span class="sxs-lookup"><span data-stu-id="11f79-133">The id of the group to remove from the policy.</span></span>|

## <a name="response"></a><span data-ttu-id="11f79-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="11f79-134">Response</span></span>

<span data-ttu-id="11f79-135">Quando é bem-sucedido, este método retorna um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="11f79-135">If successful, this method returns `200 OK` response code.</span></span> <span data-ttu-id="11f79-136">Quando o grupo é removido da política, o valor **true** é retornado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="11f79-136">If the group is removed from the policy, a **true** value is returned in the response body.</span></span> <span data-ttu-id="11f79-137">Caso contrário, um valor **false** é retornado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="11f79-137">Otherwise, a **false** value is returned in the reponse body.</span></span>

## <a name="example"></a><span data-ttu-id="11f79-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="11f79-138">Example</span></span>

##### <a name="request"></a><span data-ttu-id="11f79-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="11f79-139">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "grouplifecyclepolicy_removegroup"
} -->
```http
POST https://graph.microsoft.com/v1.0/groupLifecyclePolicies/{id}/removeGroup
Content-type: application/json
Content-length: 57

{
  "groupId": "ffffffff-ffff-ffff-ffff-ffffffffffff"
}
```

##### <a name="response"></a><span data-ttu-id="11f79-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="11f79-140">Response</span></span>
<!-- { "blockType": "response" } -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 21

{
  "value": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "groupLifecyclePolicy: removegroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

