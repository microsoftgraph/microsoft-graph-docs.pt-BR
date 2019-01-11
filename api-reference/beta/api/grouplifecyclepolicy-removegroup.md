---
title: 'groupLifecyclePolicy: removeGroup'
description: Remove um grupo de uma política de ciclo de vida.
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: faf394e411301d268a307151d98ec84a9b4e19a9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894121"
---
# <a name="grouplifecyclepolicy-removegroup"></a><span data-ttu-id="bbd38-103">groupLifecyclePolicy: removeGroup</span><span class="sxs-lookup"><span data-stu-id="bbd38-103">groupLifecyclePolicy: removeGroup</span></span>

> <span data-ttu-id="bbd38-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="bbd38-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bbd38-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="bbd38-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bbd38-106">Remove um grupo de uma política de ciclo de vida.</span><span class="sxs-lookup"><span data-stu-id="bbd38-106">Removes a group from a lifecycle policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="bbd38-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="bbd38-107">Permissions</span></span>

<span data-ttu-id="bbd38-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bbd38-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="bbd38-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bbd38-110">Permission type</span></span>      | <span data-ttu-id="bbd38-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bbd38-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bbd38-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bbd38-112">Delegated (work or school account)</span></span> | <span data-ttu-id="bbd38-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bbd38-113">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="bbd38-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bbd38-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bbd38-115">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="bbd38-115">Not supported</span></span> |
|<span data-ttu-id="bbd38-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bbd38-116">Application</span></span> |  <span data-ttu-id="bbd38-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bbd38-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bbd38-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bbd38-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies/{id}/removeGroup
```

## <a name="request-headers"></a><span data-ttu-id="bbd38-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bbd38-119">Request headers</span></span>

| <span data-ttu-id="bbd38-120">Nome</span><span class="sxs-lookup"><span data-stu-id="bbd38-120">Name</span></span> | <span data-ttu-id="bbd38-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="bbd38-121">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="bbd38-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="bbd38-122">Authorization</span></span> | <span data-ttu-id="bbd38-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bbd38-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bbd38-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bbd38-125">Content-Type</span></span>  | <span data-ttu-id="bbd38-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bbd38-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="bbd38-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bbd38-127">Request body</span></span>
<span data-ttu-id="bbd38-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bbd38-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="bbd38-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="bbd38-129">Parameter</span></span> | <span data-ttu-id="bbd38-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="bbd38-130">Type</span></span> | <span data-ttu-id="bbd38-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="bbd38-131">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="bbd38-132">groupId</span><span class="sxs-lookup"><span data-stu-id="bbd38-132">groupId</span></span>|<span data-ttu-id="bbd38-133">Guid</span><span class="sxs-lookup"><span data-stu-id="bbd38-133">Guid</span></span>| <span data-ttu-id="bbd38-134">A ID do grupo que será removido da política.</span><span class="sxs-lookup"><span data-stu-id="bbd38-134">The id of the group to remove from the policy.</span></span>|

## <a name="response"></a><span data-ttu-id="bbd38-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="bbd38-135">Response</span></span>

<span data-ttu-id="bbd38-136">Quando é bem-sucedido, este método retorna um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="bbd38-136">If successful, this method returns `200 OK` response code.</span></span> <span data-ttu-id="bbd38-137">Quando o grupo é removido da política, o valor **true** é retornado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bbd38-137">If the group is removed from the policy, a **true** value is returned in the response body.</span></span> <span data-ttu-id="bbd38-138">Caso contrário, um valor **false** é retornado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bbd38-138">Otherwise, a **false** value is returned in the reponse body.</span></span>

## <a name="example"></a><span data-ttu-id="bbd38-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bbd38-139">Example</span></span>

##### <a name="request"></a><span data-ttu-id="bbd38-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bbd38-140">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="bbd38-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="bbd38-141">Response</span></span>
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
