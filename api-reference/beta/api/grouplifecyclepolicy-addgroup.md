---
title: 'groupLifecyclePolicy: addGroup'
description: Adiciona um grupo a uma política de ciclo de vida.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: e52364353587b97e4d6cb983705d228ab93d75b3
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33328468"
---
# <a name="grouplifecyclepolicy-addgroup"></a><span data-ttu-id="b34f5-103">groupLifecyclePolicy: addGroup</span><span class="sxs-lookup"><span data-stu-id="b34f5-103">groupLifecyclePolicy: addGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b34f5-104">Adiciona um grupo a uma política de ciclo de vida.</span><span class="sxs-lookup"><span data-stu-id="b34f5-104">Adds a group to a lifecycle policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="b34f5-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="b34f5-105">Permissions</span></span>

<span data-ttu-id="b34f5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b34f5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="b34f5-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b34f5-108">Permission type</span></span>      | <span data-ttu-id="b34f5-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b34f5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b34f5-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b34f5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b34f5-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b34f5-111">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="b34f5-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b34f5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b34f5-113">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="b34f5-113">Not supported</span></span> |
|<span data-ttu-id="b34f5-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b34f5-114">Application</span></span> | <span data-ttu-id="b34f5-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b34f5-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b34f5-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b34f5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies/{id}/addGroup
```

## <a name="request-headers"></a><span data-ttu-id="b34f5-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b34f5-117">Request headers</span></span>

| <span data-ttu-id="b34f5-118">Nome</span><span class="sxs-lookup"><span data-stu-id="b34f5-118">Name</span></span> | <span data-ttu-id="b34f5-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="b34f5-119">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="b34f5-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="b34f5-120">Authorization</span></span> | <span data-ttu-id="b34f5-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b34f5-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b34f5-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b34f5-123">Content-Type</span></span>  | <span data-ttu-id="b34f5-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b34f5-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="b34f5-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b34f5-125">Request body</span></span>
<span data-ttu-id="b34f5-126">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b34f5-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b34f5-127">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="b34f5-127">Parameter</span></span> | <span data-ttu-id="b34f5-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="b34f5-128">Type</span></span> | <span data-ttu-id="b34f5-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="b34f5-129">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="b34f5-130">groupId</span><span class="sxs-lookup"><span data-stu-id="b34f5-130">groupId</span></span>|<span data-ttu-id="b34f5-131">Guid</span><span class="sxs-lookup"><span data-stu-id="b34f5-131">Guid</span></span>| <span data-ttu-id="b34f5-132">A ID do grupo que será adicionado à política.</span><span class="sxs-lookup"><span data-stu-id="b34f5-132">The id of the group to add to the policy.</span></span> |

## <a name="response"></a><span data-ttu-id="b34f5-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="b34f5-133">Response</span></span>

<span data-ttu-id="b34f5-134">Quando é bem-sucedido, este método retorna um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="b34f5-134">If successful, this method returns `200 OK` response code.</span></span> <span data-ttu-id="b34f5-135">Quando o grupo é adicionado à política, o valor **true** é retornado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b34f5-135">If the group is added to the policy, a **true** value is returned in the response body.</span></span> <span data-ttu-id="b34f5-136">Caso contrário, um valor **false** é retornado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b34f5-136">Otherwise, a **false** value is returned in the reponse body.</span></span>

## <a name="example"></a><span data-ttu-id="b34f5-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b34f5-137">Example</span></span>

#### <a name="request"></a><span data-ttu-id="b34f5-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b34f5-138">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="b34f5-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="b34f5-139">Response</span></span>
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
