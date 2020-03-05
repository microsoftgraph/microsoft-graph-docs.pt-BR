---
title: 'groupLifecyclePolicy: removeGroup'
description: Remove um grupo de uma política de ciclo de vida.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 05c2b5180c3de75df29e7733480c43b26406725b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446583"
---
# <a name="grouplifecyclepolicy-removegroup"></a><span data-ttu-id="957ef-103">groupLifecyclePolicy: removeGroup</span><span class="sxs-lookup"><span data-stu-id="957ef-103">groupLifecyclePolicy: removeGroup</span></span>

<span data-ttu-id="957ef-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="957ef-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="957ef-105">Remove um grupo de uma política de ciclo de vida.</span><span class="sxs-lookup"><span data-stu-id="957ef-105">Removes a group from a lifecycle policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="957ef-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="957ef-106">Permissions</span></span>

<span data-ttu-id="957ef-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="957ef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="957ef-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="957ef-109">Permission type</span></span>      | <span data-ttu-id="957ef-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="957ef-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="957ef-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="957ef-111">Delegated (work or school account)</span></span> | <span data-ttu-id="957ef-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="957ef-112">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="957ef-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="957ef-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="957ef-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="957ef-114">Not supported</span></span> |
|<span data-ttu-id="957ef-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="957ef-115">Application</span></span> |  <span data-ttu-id="957ef-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="957ef-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="957ef-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="957ef-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies/{id}/removeGroup
```

## <a name="request-headers"></a><span data-ttu-id="957ef-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="957ef-118">Request headers</span></span>

| <span data-ttu-id="957ef-119">Nome</span><span class="sxs-lookup"><span data-stu-id="957ef-119">Name</span></span> | <span data-ttu-id="957ef-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="957ef-120">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="957ef-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="957ef-121">Authorization</span></span> | <span data-ttu-id="957ef-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="957ef-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="957ef-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="957ef-124">Content-Type</span></span>  | <span data-ttu-id="957ef-125">application/json</span><span class="sxs-lookup"><span data-stu-id="957ef-125">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="957ef-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="957ef-126">Request body</span></span>
<span data-ttu-id="957ef-127">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="957ef-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="957ef-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="957ef-128">Parameter</span></span> | <span data-ttu-id="957ef-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="957ef-129">Type</span></span> | <span data-ttu-id="957ef-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="957ef-130">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="957ef-131">groupId</span><span class="sxs-lookup"><span data-stu-id="957ef-131">groupId</span></span>|<span data-ttu-id="957ef-132">Guid</span><span class="sxs-lookup"><span data-stu-id="957ef-132">Guid</span></span>| <span data-ttu-id="957ef-133">A ID do grupo que será removido da política.</span><span class="sxs-lookup"><span data-stu-id="957ef-133">The id of the group to remove from the policy.</span></span>|

## <a name="response"></a><span data-ttu-id="957ef-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="957ef-134">Response</span></span>

<span data-ttu-id="957ef-135">Se bem sucedido, este método retorna um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="957ef-135">If successful, this method returns `200 OK` response code.</span></span> <span data-ttu-id="957ef-136">Quando o grupo é removido da política, o valor **true** é retornado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="957ef-136">If the group is removed from the policy, a **true** value is returned in the response body.</span></span> <span data-ttu-id="957ef-137">Caso contrário, um valor **false** é retornado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="957ef-137">Otherwise, a **false** value is returned in the reponse body.</span></span>

## <a name="example"></a><span data-ttu-id="957ef-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="957ef-138">Example</span></span>

##### <a name="request"></a><span data-ttu-id="957ef-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="957ef-139">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "grouplifecyclepolicy_removegroup"
} -->
```http
POST https://graph.microsoft.com/beta/groupLifecyclePolicies/{id}/removeGroup
Content-type: application/json
Content-length: 57

{
  "groupId": "ffffffff-ffff-ffff-ffff-ffffffffffff"
}
```

##### <a name="response"></a><span data-ttu-id="957ef-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="957ef-140">Response</span></span>
<!-- { "blockType": "ignored" } -->

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
<!--
{
  "type": "#page.annotation",
  "description": "groupLifecyclePolicy: removegroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
