---
title: 'groupLifecyclePolicy: removeGroup'
description: Remove um grupo de uma política de ciclo de vida.
author: Jordanndahl
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: e081dcbfa268999598c8cfa13b4cd1acd53ec6ee
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2021
ms.locfileid: "53316668"
---
# <a name="grouplifecyclepolicy-removegroup"></a><span data-ttu-id="f559a-103">groupLifecyclePolicy: removeGroup</span><span class="sxs-lookup"><span data-stu-id="f559a-103">groupLifecyclePolicy: removeGroup</span></span>

<span data-ttu-id="f559a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f559a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f559a-105">Remove um grupo de uma política de ciclo de vida.</span><span class="sxs-lookup"><span data-stu-id="f559a-105">Removes a group from a lifecycle policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="f559a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f559a-106">Permissions</span></span>

<span data-ttu-id="f559a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f559a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="f559a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f559a-109">Permission type</span></span>      | <span data-ttu-id="f559a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f559a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f559a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f559a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f559a-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f559a-112">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="f559a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f559a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f559a-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="f559a-114">Not supported</span></span> |
|<span data-ttu-id="f559a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f559a-115">Application</span></span> |  <span data-ttu-id="f559a-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f559a-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f559a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f559a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies/{id}/removeGroup
```

## <a name="request-headers"></a><span data-ttu-id="f559a-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f559a-118">Request headers</span></span>

| <span data-ttu-id="f559a-119">Nome</span><span class="sxs-lookup"><span data-stu-id="f559a-119">Name</span></span> | <span data-ttu-id="f559a-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="f559a-120">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="f559a-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="f559a-121">Authorization</span></span> | <span data-ttu-id="f559a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f559a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f559a-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f559a-124">Content-Type</span></span>  | <span data-ttu-id="f559a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f559a-125">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="f559a-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f559a-126">Request body</span></span>
<span data-ttu-id="f559a-127">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f559a-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f559a-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="f559a-128">Parameter</span></span> | <span data-ttu-id="f559a-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="f559a-129">Type</span></span> | <span data-ttu-id="f559a-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="f559a-130">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="f559a-131">groupId</span><span class="sxs-lookup"><span data-stu-id="f559a-131">groupId</span></span>|<span data-ttu-id="f559a-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f559a-132">String</span></span>| <span data-ttu-id="f559a-133">O identificador do grupo a ser removido da política.</span><span class="sxs-lookup"><span data-stu-id="f559a-133">The identifier of the group to remove from the policy.</span></span>|

## <a name="response"></a><span data-ttu-id="f559a-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="f559a-134">Response</span></span>

<span data-ttu-id="f559a-135">Se bem sucedido, este método retorna um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="f559a-135">If successful, this method returns `200 OK` response code.</span></span> <span data-ttu-id="f559a-136">Se o grupo for removido da política, um `true` valor será retornado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f559a-136">If the group is removed from the policy, a `true` value is returned in the response body.</span></span> <span data-ttu-id="f559a-137">Caso contrário, `false` um valor será retornado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f559a-137">Otherwise, a `false` value is returned in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f559a-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f559a-138">Example</span></span>

##### <a name="request"></a><span data-ttu-id="f559a-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f559a-139">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="f559a-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="f559a-140">Response</span></span>
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


