---
title: 'groupLifecyclePolicy: addGroup'
description: Adiciona um grupo a uma política de ciclo de vida.
author: Jordanndahl
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 07fc0bb3c1d26aedecbc49fd839fe3801c9d6651
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2021
ms.locfileid: "53316997"
---
# <a name="grouplifecyclepolicy-addgroup"></a><span data-ttu-id="3991f-103">groupLifecyclePolicy: addGroup</span><span class="sxs-lookup"><span data-stu-id="3991f-103">groupLifecyclePolicy: addGroup</span></span>

<span data-ttu-id="3991f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3991f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3991f-105">Adiciona grupos específicos a uma política de ciclo de vida.</span><span class="sxs-lookup"><span data-stu-id="3991f-105">Adds specific groups to a lifecycle policy.</span></span> <span data-ttu-id="3991f-106">Essa ação limita a política de ciclo de vida do grupo a um conjunto de grupos somente se a propriedade **managedGroupTypes** do [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) estiver definida como `Selected` .</span><span class="sxs-lookup"><span data-stu-id="3991f-106">This action limits the group lifecycle policy to a set of groups only if the **managedGroupTypes** property of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) is set to `Selected`.</span></span>

## <a name="permissions"></a><span data-ttu-id="3991f-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="3991f-107">Permissions</span></span>

<span data-ttu-id="3991f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3991f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="3991f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3991f-110">Permission type</span></span>      | <span data-ttu-id="3991f-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3991f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3991f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3991f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3991f-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3991f-113">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="3991f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3991f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3991f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3991f-115">Not supported.</span></span>    |
|<span data-ttu-id="3991f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3991f-116">Application</span></span> | <span data-ttu-id="3991f-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3991f-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3991f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3991f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies/{id}/addGroup
```

## <a name="request-headers"></a><span data-ttu-id="3991f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3991f-119">Request headers</span></span>

| <span data-ttu-id="3991f-120">Nome</span><span class="sxs-lookup"><span data-stu-id="3991f-120">Name</span></span> | <span data-ttu-id="3991f-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="3991f-121">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="3991f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="3991f-122">Authorization</span></span> | <span data-ttu-id="3991f-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3991f-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3991f-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3991f-125">Content-Type</span></span>  | <span data-ttu-id="3991f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3991f-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="3991f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3991f-127">Request body</span></span>
<span data-ttu-id="3991f-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3991f-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="3991f-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="3991f-129">Parameter</span></span> | <span data-ttu-id="3991f-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="3991f-130">Type</span></span> | <span data-ttu-id="3991f-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="3991f-131">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="3991f-132">groupId</span><span class="sxs-lookup"><span data-stu-id="3991f-132">groupId</span></span>|<span data-ttu-id="3991f-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3991f-133">String</span></span>| <span data-ttu-id="3991f-134">O identificador do grupo a ser acrescentado à política.</span><span class="sxs-lookup"><span data-stu-id="3991f-134">The identifier of the group to add to the policy.</span></span> |

<span data-ttu-id="3991f-135">Quando a **propriedade managedGroupTypes** [do groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) é definida como , você pode adicionar até `Selected` 500 grupos à lista.</span><span class="sxs-lookup"><span data-stu-id="3991f-135">When the **managedGroupTypes** property of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) is set to `Selected`, you can add up to 500 groups to the list.</span></span> <span data-ttu-id="3991f-136">Se você precisar adicionar mais de 500 grupos, a propriedade **managedGroupTypes** do [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) deve ser definida como `All` .</span><span class="sxs-lookup"><span data-stu-id="3991f-136">If you need to add more than 500 groups, the **managedGroupTypes** property of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) must be set to `All`.</span></span>

<span data-ttu-id="3991f-137">Somente um grupo pode ser adicionado por solicitação.</span><span class="sxs-lookup"><span data-stu-id="3991f-137">Only one group can be added per request.</span></span>

## <a name="response"></a><span data-ttu-id="3991f-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="3991f-138">Response</span></span>

<span data-ttu-id="3991f-139">Se bem sucedido, este método retorna um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="3991f-139">If successful, this method returns `200 OK` response code.</span></span> <span data-ttu-id="3991f-140">Se o grupo for adicionado à política, um `true` valor será retornado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3991f-140">If the group is added to the policy, a `true` value is returned in the response body.</span></span> <span data-ttu-id="3991f-141">Caso contrário, `false` um valor será retornado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3991f-141">Otherwise, a `false` value is returned in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3991f-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3991f-142">Example</span></span>

#### <a name="request"></a><span data-ttu-id="3991f-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3991f-143">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "grouplifecyclepolicy_addgroup"
} -->
```http
POST https://graph.microsoft.com/v1.0/groupLifecyclePolicies/{id}/addGroup
Content-type: application/json
Content-length: 57

{
  "groupId": "ffffffff-ffff-ffff-ffff-ffffffffffff"
}
```

#### <a name="response"></a><span data-ttu-id="3991f-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="3991f-144">Response</span></span>
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

