---
title: 'groupLifecyclePolicy: addGroup'
description: Adiciona um grupo a uma política de ciclo de vida.
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: ac0bf455ba2d4aa5f1f6add5827124581ce663b5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27853358"
---
# <a name="grouplifecyclepolicy-addgroup"></a><span data-ttu-id="d5960-103">groupLifecyclePolicy: addGroup</span><span class="sxs-lookup"><span data-stu-id="d5960-103">groupLifecyclePolicy: addGroup</span></span>

> <span data-ttu-id="d5960-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d5960-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d5960-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d5960-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d5960-106">Adiciona um grupo a uma política de ciclo de vida.</span><span class="sxs-lookup"><span data-stu-id="d5960-106">Adds a group to a lifecycle policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="d5960-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="d5960-107">Permissions</span></span>

<span data-ttu-id="d5960-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d5960-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d5960-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d5960-110">Permission type</span></span>      | <span data-ttu-id="d5960-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d5960-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d5960-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d5960-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d5960-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5960-113">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="d5960-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d5960-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d5960-115">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="d5960-115">Not supported</span></span> |
|<span data-ttu-id="d5960-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d5960-116">Application</span></span> | <span data-ttu-id="d5960-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5960-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d5960-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d5960-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies/{id}/addGroup
```

## <a name="request-headers"></a><span data-ttu-id="d5960-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d5960-119">Request headers</span></span>

| <span data-ttu-id="d5960-120">Nome</span><span class="sxs-lookup"><span data-stu-id="d5960-120">Name</span></span> | <span data-ttu-id="d5960-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5960-121">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="d5960-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d5960-122">Authorization</span></span> | <span data-ttu-id="d5960-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d5960-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d5960-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d5960-125">Content-Type</span></span>  | <span data-ttu-id="d5960-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d5960-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="d5960-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d5960-127">Request body</span></span>
<span data-ttu-id="d5960-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d5960-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d5960-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="d5960-129">Parameter</span></span> | <span data-ttu-id="d5960-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="d5960-130">Type</span></span> | <span data-ttu-id="d5960-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5960-131">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="d5960-132">groupId</span><span class="sxs-lookup"><span data-stu-id="d5960-132">groupId</span></span>|<span data-ttu-id="d5960-133">Guid</span><span class="sxs-lookup"><span data-stu-id="d5960-133">Guid</span></span>| <span data-ttu-id="d5960-134">A ID do grupo que será adicionado à política.</span><span class="sxs-lookup"><span data-stu-id="d5960-134">The id of the group to add to the policy.</span></span> |

## <a name="response"></a><span data-ttu-id="d5960-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="d5960-135">Response</span></span>

<span data-ttu-id="d5960-136">Quando é bem-sucedido, este método retorna um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="d5960-136">If successful, this method returns `200 OK` response code.</span></span> <span data-ttu-id="d5960-137">Quando o grupo é adicionado à política, o valor **true** é retornado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d5960-137">If the group is added to the policy, a **true** value is returned in the response body.</span></span> <span data-ttu-id="d5960-138">Caso contrário, um valor **false** é retornado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d5960-138">Otherwise, a **false** value is returned in the reponse body.</span></span>

## <a name="example"></a><span data-ttu-id="d5960-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d5960-139">Example</span></span>

#### <a name="request"></a><span data-ttu-id="d5960-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d5960-140">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="d5960-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="d5960-141">Response</span></span>
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
  "description": "groupLifecyclePolicy: addgroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
