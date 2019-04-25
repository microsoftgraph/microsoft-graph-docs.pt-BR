---
title: 'groupLifecyclePolicy: removeGroup'
description: Remove um grupo de uma política de ciclo de vida.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 7affc1af4fcee76cfa4ff044bc11604247d46762
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32525702"
---
# <a name="grouplifecyclepolicy-removegroup"></a><span data-ttu-id="a6684-103">groupLifecyclePolicy: removeGroup</span><span class="sxs-lookup"><span data-stu-id="a6684-103">groupLifecyclePolicy: removeGroup</span></span>

<span data-ttu-id="a6684-104">Remove um grupo de uma política de ciclo de vida.</span><span class="sxs-lookup"><span data-stu-id="a6684-104">Removes a group from a lifecycle policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="a6684-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="a6684-105">Permissions</span></span>

<span data-ttu-id="a6684-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a6684-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6684-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a6684-108">Permission type</span></span>      | <span data-ttu-id="a6684-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a6684-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a6684-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a6684-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a6684-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6684-111">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="a6684-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a6684-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a6684-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a6684-113">Not supported.</span></span>    |
|<span data-ttu-id="a6684-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a6684-114">Application</span></span> | <span data-ttu-id="a6684-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6684-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a6684-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a6684-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies/{id}/removeGroup
```

## <a name="request-headers"></a><span data-ttu-id="a6684-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a6684-117">Request headers</span></span>

| <span data-ttu-id="a6684-118">Nome</span><span class="sxs-lookup"><span data-stu-id="a6684-118">Name</span></span> | <span data-ttu-id="a6684-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="a6684-119">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="a6684-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="a6684-120">Authorization</span></span> | <span data-ttu-id="a6684-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a6684-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a6684-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a6684-123">Content-Type</span></span>  | <span data-ttu-id="a6684-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a6684-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="a6684-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a6684-125">Request body</span></span>
<span data-ttu-id="a6684-126">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a6684-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a6684-127">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="a6684-127">Parameter</span></span> | <span data-ttu-id="a6684-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="a6684-128">Type</span></span> | <span data-ttu-id="a6684-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="a6684-129">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="a6684-130">groupId</span><span class="sxs-lookup"><span data-stu-id="a6684-130">groupId</span></span>|<span data-ttu-id="a6684-131">Guid</span><span class="sxs-lookup"><span data-stu-id="a6684-131">Guid</span></span>| <span data-ttu-id="a6684-132">A ID do grupo que será removido da política.</span><span class="sxs-lookup"><span data-stu-id="a6684-132">The id of the group to remove from the policy.</span></span>|

## <a name="response"></a><span data-ttu-id="a6684-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6684-133">Response</span></span>

<span data-ttu-id="a6684-134">Quando é bem-sucedido, este método retorna um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="a6684-134">If successful, this method returns `200 OK` response code.</span></span> <span data-ttu-id="a6684-135">Quando o grupo é removido da política, o valor **true** é retornado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a6684-135">If the group is removed from the policy, a **true** value is returned in the response body.</span></span> <span data-ttu-id="a6684-136">Caso contrário, um valor **false** é retornado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a6684-136">Otherwise, a **false** value is returned in the reponse body.</span></span>

## <a name="example"></a><span data-ttu-id="a6684-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a6684-137">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a6684-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a6684-138">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="a6684-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6684-139">Response</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "groupLifecyclePolicy: removegroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
