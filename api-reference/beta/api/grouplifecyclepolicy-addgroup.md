---
title: 'groupLifecyclePolicy: addGroup'
description: Adiciona um grupo a uma política de ciclo de vida.
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 2bea2b06f4d016859a4fb482dfb32dd8a1365eca
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/03/2020
ms.locfileid: "43123710"
---
# <a name="grouplifecyclepolicy-addgroup"></a><span data-ttu-id="02c50-103">groupLifecyclePolicy: addGroup</span><span class="sxs-lookup"><span data-stu-id="02c50-103">groupLifecyclePolicy: addGroup</span></span>

<span data-ttu-id="02c50-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="02c50-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="02c50-105">Adiciona um grupo a uma política de ciclo de vida.</span><span class="sxs-lookup"><span data-stu-id="02c50-105">Adds a group to a lifecycle policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="02c50-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="02c50-106">Permissions</span></span>

<span data-ttu-id="02c50-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02c50-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="02c50-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="02c50-109">Permission type</span></span>      | <span data-ttu-id="02c50-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="02c50-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="02c50-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="02c50-111">Delegated (work or school account)</span></span> | <span data-ttu-id="02c50-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02c50-112">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="02c50-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="02c50-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="02c50-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="02c50-114">Not supported</span></span> |
|<span data-ttu-id="02c50-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="02c50-115">Application</span></span> | <span data-ttu-id="02c50-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02c50-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="02c50-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="02c50-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies/{id}/addGroup
```

## <a name="request-headers"></a><span data-ttu-id="02c50-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="02c50-118">Request headers</span></span>

| <span data-ttu-id="02c50-119">Nome</span><span class="sxs-lookup"><span data-stu-id="02c50-119">Name</span></span> | <span data-ttu-id="02c50-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="02c50-120">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="02c50-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="02c50-121">Authorization</span></span> | <span data-ttu-id="02c50-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="02c50-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="02c50-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="02c50-124">Content-Type</span></span>  | <span data-ttu-id="02c50-125">application/json</span><span class="sxs-lookup"><span data-stu-id="02c50-125">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="02c50-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="02c50-126">Request body</span></span>
<span data-ttu-id="02c50-127">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="02c50-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="02c50-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="02c50-128">Parameter</span></span> | <span data-ttu-id="02c50-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="02c50-129">Type</span></span> | <span data-ttu-id="02c50-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="02c50-130">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="02c50-131">groupId</span><span class="sxs-lookup"><span data-stu-id="02c50-131">groupId</span></span>|<span data-ttu-id="02c50-132">Guid</span><span class="sxs-lookup"><span data-stu-id="02c50-132">Guid</span></span>| <span data-ttu-id="02c50-133">A ID do grupo que será adicionado à política.</span><span class="sxs-lookup"><span data-stu-id="02c50-133">The id of the group to add to the policy.</span></span> |

## <a name="response"></a><span data-ttu-id="02c50-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="02c50-134">Response</span></span>

<span data-ttu-id="02c50-135">Se bem sucedido, este método retorna um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="02c50-135">If successful, this method returns `200 OK` response code.</span></span> <span data-ttu-id="02c50-136">Quando o grupo é adicionado à política, o valor **true** é retornado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="02c50-136">If the group is added to the policy, a **true** value is returned in the response body.</span></span> <span data-ttu-id="02c50-137">Caso contrário, um valor **false** é retornado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="02c50-137">Otherwise, a **false** value is returned in the reponse body.</span></span>

## <a name="example"></a><span data-ttu-id="02c50-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="02c50-138">Example</span></span>

#### <a name="request"></a><span data-ttu-id="02c50-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="02c50-139">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="02c50-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="02c50-140">Response</span></span>
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
