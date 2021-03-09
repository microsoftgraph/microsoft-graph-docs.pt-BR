---
title: 'user: activateServicePlan'
description: Ative um plano de serviço com um `servicePlanId` determinado e para um determinado `skuId` usuário.
author: dkershaw10
localization_priority: Normal
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 70849865237a82f4a0bb5fcee22263291627c21d
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50578851"
---
# <a name="user-activateserviceplan"></a><span data-ttu-id="09441-103">user: activateServicePlan</span><span class="sxs-lookup"><span data-stu-id="09441-103">user: activateServicePlan</span></span>

<span data-ttu-id="09441-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="09441-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="09441-105">Ative um plano de serviço com um `servicePlanId` determinado e para um determinado `skuId` usuário.</span><span class="sxs-lookup"><span data-stu-id="09441-105">Activate a service plan with a given `servicePlanId` and `skuId` for a given user.</span></span>

## <a name="permissions"></a><span data-ttu-id="09441-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="09441-106">Permissions</span></span>

<span data-ttu-id="09441-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="09441-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="09441-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="09441-109">Permission type</span></span>|<span data-ttu-id="09441-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="09441-110">Permissions (from most to least privileged)</span></span>|
| :--- | :--- |
| <span data-ttu-id="09441-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="09441-111">Delegated (work or school account)</span></span> | <span data-ttu-id="09441-112">Directory.ReadWrite.All, Directory.ReadWriteAdvanced.All</span><span class="sxs-lookup"><span data-stu-id="09441-112">Directory.ReadWrite.All, Directory.ReadWriteAdvanced.All</span></span> |
| <span data-ttu-id="09441-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="09441-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="09441-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="09441-114">Not Supported.</span></span> |
| <span data-ttu-id="09441-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="09441-115">Application</span></span> | <span data-ttu-id="09441-116">Directory.ReadWrite.All, Directory.ReadWriteAdvanced.All</span><span class="sxs-lookup"><span data-stu-id="09441-116">Directory.ReadWrite.All, Directory.ReadWriteAdvanced.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="09441-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="09441-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /users/{id | userPrincipalName}/activateServicePlan
```

## <a name="request-headers"></a><span data-ttu-id="09441-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="09441-118">Request headers</span></span>

| <span data-ttu-id="09441-119">Nome</span><span class="sxs-lookup"><span data-stu-id="09441-119">Name</span></span> | <span data-ttu-id="09441-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="09441-120">Description</span></span> |
| :--- | :--- |
| <span data-ttu-id="09441-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="09441-121">Authorization</span></span> | <span data-ttu-id="09441-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="09441-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="09441-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="09441-124">Content-Type</span></span> | <span data-ttu-id="09441-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="09441-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="09441-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="09441-127">Request body</span></span>

<span data-ttu-id="09441-128">No corpo da solicitação, forneça um objeto JSON com o seguinte parâmetro:</span><span class="sxs-lookup"><span data-stu-id="09441-128">In the request body, provide a JSON object with the following parameter:</span></span>

| <span data-ttu-id="09441-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="09441-129">Parameter</span></span> | <span data-ttu-id="09441-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="09441-130">Type</span></span> | <span data-ttu-id="09441-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="09441-131">Description</span></span> |
| :--- | :--- | :--- |
| <span data-ttu-id="09441-132">servicePlanId</span><span class="sxs-lookup"><span data-stu-id="09441-132">servicePlanId</span></span> | <span data-ttu-id="09441-133">Guid</span><span class="sxs-lookup"><span data-stu-id="09441-133">Guid</span></span> | <span data-ttu-id="09441-134">PlanId do ServicePlan a ser ativado.</span><span class="sxs-lookup"><span data-stu-id="09441-134">PlanId of the ServicePlan to activate.</span></span> |
| <span data-ttu-id="09441-135">skuId</span><span class="sxs-lookup"><span data-stu-id="09441-135">skuId</span></span> | <span data-ttu-id="09441-136">Guid</span><span class="sxs-lookup"><span data-stu-id="09441-136">Guid</span></span> | <span data-ttu-id="09441-137">SkuId de SKU o plano de serviço está em.</span><span class="sxs-lookup"><span data-stu-id="09441-137">SkuId of SKU the service plan is on.</span></span> |

## <a name="response"></a><span data-ttu-id="09441-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="09441-138">Response</span></span>

<span data-ttu-id="09441-139">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="09441-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="09441-140">Exemplos</span><span class="sxs-lookup"><span data-stu-id="09441-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="09441-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="09441-141">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "user_activateserviceplan"
}
-->

``` http
POST https://graph.microsoft.com/beta/me/activateServicePlan
Content-type: application/json
Content-length: 115

{
  "servicePlanId": "28f42d6f-8034-4a0f-9d8a-a218a63b3299",
  "skuId": "465a2a90-5e59-456d-a7b8-127b9fb2e484"
}
```

### <a name="response"></a><span data-ttu-id="09441-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="09441-142">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
