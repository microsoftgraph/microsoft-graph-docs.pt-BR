---
title: 'groupLifecyclePolicy: addGroup'
description: Adiciona um grupo a uma política de ciclo de vida.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 07ad966a3fbbfd6a44fc5a744366d8e7d754e5be
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446608"
---
# <a name="grouplifecyclepolicy-addgroup"></a><span data-ttu-id="55c0f-103">groupLifecyclePolicy: addGroup</span><span class="sxs-lookup"><span data-stu-id="55c0f-103">groupLifecyclePolicy: addGroup</span></span>

<span data-ttu-id="55c0f-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="55c0f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="55c0f-105">Adiciona um grupo a uma política de ciclo de vida.</span><span class="sxs-lookup"><span data-stu-id="55c0f-105">Adds a group to a lifecycle policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="55c0f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="55c0f-106">Permissions</span></span>

<span data-ttu-id="55c0f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="55c0f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="55c0f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="55c0f-109">Permission type</span></span>      | <span data-ttu-id="55c0f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="55c0f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="55c0f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="55c0f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="55c0f-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55c0f-112">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="55c0f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="55c0f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="55c0f-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="55c0f-114">Not supported</span></span> |
|<span data-ttu-id="55c0f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="55c0f-115">Application</span></span> | <span data-ttu-id="55c0f-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55c0f-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="55c0f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="55c0f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies/{id}/addGroup
```

## <a name="request-headers"></a><span data-ttu-id="55c0f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="55c0f-118">Request headers</span></span>

| <span data-ttu-id="55c0f-119">Nome</span><span class="sxs-lookup"><span data-stu-id="55c0f-119">Name</span></span> | <span data-ttu-id="55c0f-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="55c0f-120">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="55c0f-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="55c0f-121">Authorization</span></span> | <span data-ttu-id="55c0f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="55c0f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="55c0f-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="55c0f-124">Content-Type</span></span>  | <span data-ttu-id="55c0f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="55c0f-125">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="55c0f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="55c0f-126">Request body</span></span>
<span data-ttu-id="55c0f-127">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="55c0f-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="55c0f-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="55c0f-128">Parameter</span></span> | <span data-ttu-id="55c0f-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="55c0f-129">Type</span></span> | <span data-ttu-id="55c0f-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="55c0f-130">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="55c0f-131">groupId</span><span class="sxs-lookup"><span data-stu-id="55c0f-131">groupId</span></span>|<span data-ttu-id="55c0f-132">Guid</span><span class="sxs-lookup"><span data-stu-id="55c0f-132">Guid</span></span>| <span data-ttu-id="55c0f-133">A ID do grupo que será adicionado à política.</span><span class="sxs-lookup"><span data-stu-id="55c0f-133">The id of the group to add to the policy.</span></span> |

## <a name="response"></a><span data-ttu-id="55c0f-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="55c0f-134">Response</span></span>

<span data-ttu-id="55c0f-135">Se bem sucedido, este método retorna um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="55c0f-135">If successful, this method returns `200 OK` response code.</span></span> <span data-ttu-id="55c0f-136">Quando o grupo é adicionado à política, o valor **true** é retornado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="55c0f-136">If the group is added to the policy, a **true** value is returned in the response body.</span></span> <span data-ttu-id="55c0f-137">Caso contrário, um valor **false** é retornado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="55c0f-137">Otherwise, a **false** value is returned in the reponse body.</span></span>

## <a name="example"></a><span data-ttu-id="55c0f-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="55c0f-138">Example</span></span>

#### <a name="request"></a><span data-ttu-id="55c0f-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="55c0f-139">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "grouplifecyclepolicy_addgroup"
} -->
```http
POST https://graph.microsoft.com/beta/groupLifecyclePolicies/{id}/addGroup
Content-type: application/json
Content-length: 57

{
  "groupId": "ffffffff-ffff-ffff-ffff-ffffffffffff"
}
```

#### <a name="response"></a><span data-ttu-id="55c0f-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="55c0f-140">Response</span></span>
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
  "description": "groupLifecyclePolicy: addgroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
