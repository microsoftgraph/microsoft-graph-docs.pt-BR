---
title: 'groupLifecyclePolicy: removeGroup'
description: Remove um grupo de uma política de ciclo de vida.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 8043119b2480f0116566d668b440e4d493ebbeb5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35953308"
---
# <a name="grouplifecyclepolicy-removegroup"></a><span data-ttu-id="17b55-103">groupLifecyclePolicy: removeGroup</span><span class="sxs-lookup"><span data-stu-id="17b55-103">groupLifecyclePolicy: removeGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="17b55-104">Remove um grupo de uma política de ciclo de vida.</span><span class="sxs-lookup"><span data-stu-id="17b55-104">Removes a group from a lifecycle policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="17b55-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="17b55-105">Permissions</span></span>

<span data-ttu-id="17b55-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="17b55-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="17b55-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="17b55-108">Permission type</span></span>      | <span data-ttu-id="17b55-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="17b55-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="17b55-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="17b55-110">Delegated (work or school account)</span></span> | <span data-ttu-id="17b55-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17b55-111">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="17b55-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="17b55-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="17b55-113">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="17b55-113">Not supported</span></span> |
|<span data-ttu-id="17b55-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="17b55-114">Application</span></span> |  <span data-ttu-id="17b55-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17b55-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="17b55-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="17b55-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies/{id}/removeGroup
```

## <a name="request-headers"></a><span data-ttu-id="17b55-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="17b55-117">Request headers</span></span>

| <span data-ttu-id="17b55-118">Nome</span><span class="sxs-lookup"><span data-stu-id="17b55-118">Name</span></span> | <span data-ttu-id="17b55-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="17b55-119">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="17b55-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="17b55-120">Authorization</span></span> | <span data-ttu-id="17b55-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="17b55-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="17b55-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="17b55-123">Content-Type</span></span>  | <span data-ttu-id="17b55-124">application/json</span><span class="sxs-lookup"><span data-stu-id="17b55-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="17b55-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="17b55-125">Request body</span></span>
<span data-ttu-id="17b55-126">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="17b55-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="17b55-127">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="17b55-127">Parameter</span></span> | <span data-ttu-id="17b55-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="17b55-128">Type</span></span> | <span data-ttu-id="17b55-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="17b55-129">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="17b55-130">groupId</span><span class="sxs-lookup"><span data-stu-id="17b55-130">groupId</span></span>|<span data-ttu-id="17b55-131">Guid</span><span class="sxs-lookup"><span data-stu-id="17b55-131">Guid</span></span>| <span data-ttu-id="17b55-132">A ID do grupo que será removido da política.</span><span class="sxs-lookup"><span data-stu-id="17b55-132">The id of the group to remove from the policy.</span></span>|

## <a name="response"></a><span data-ttu-id="17b55-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="17b55-133">Response</span></span>

<span data-ttu-id="17b55-134">Quando é bem-sucedido, este método retorna um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="17b55-134">If successful, this method returns `200 OK` response code.</span></span> <span data-ttu-id="17b55-135">Quando o grupo é removido da política, o valor **true** é retornado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="17b55-135">If the group is removed from the policy, a **true** value is returned in the response body.</span></span> <span data-ttu-id="17b55-136">Caso contrário, um valor **false** é retornado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="17b55-136">Otherwise, a **false** value is returned in the reponse body.</span></span>

## <a name="example"></a><span data-ttu-id="17b55-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="17b55-137">Example</span></span>

##### <a name="request"></a><span data-ttu-id="17b55-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="17b55-138">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="17b55-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="17b55-139">Response</span></span>
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
