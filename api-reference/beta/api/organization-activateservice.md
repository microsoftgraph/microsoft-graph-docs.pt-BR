---
title: 'organization: activateService'
description: Ativa um serviço para uma organização.
author: dkershaw10
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 6008b7f5a597af5ac65b349af22879b9db1255f4
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2021
ms.locfileid: "53109073"
---
# <a name="organization-activateservice"></a><span data-ttu-id="6f842-103">organization: activateService</span><span class="sxs-lookup"><span data-stu-id="6f842-103">organization: activateService</span></span>

<span data-ttu-id="6f842-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6f842-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6f842-105">Ative um serviço para uma organização.</span><span class="sxs-lookup"><span data-stu-id="6f842-105">Activate a service for an organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="6f842-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6f842-106">Permissions</span></span>
<span data-ttu-id="6f842-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6f842-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="6f842-109">Para ativar um serviço para uma organização, o  solicitante precisa ter a função administrador da empresa com as seguintes permissões.</span><span class="sxs-lookup"><span data-stu-id="6f842-109">In order to activate a service for an organization the requestor needs to have the _Company Administrator_ role with the following permissions.</span></span>

|<span data-ttu-id="6f842-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6f842-110">Permission type</span></span>|<span data-ttu-id="6f842-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6f842-111">Permissions (from least to most privileged)</span></span>|
| :--- | :--- |
| <span data-ttu-id="6f842-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6f842-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6f842-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f842-113">Directory.ReadWrite.All</span></span>|
| <span data-ttu-id="6f842-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6f842-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6f842-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6f842-115">Not Supported.</span></span> |
| <span data-ttu-id="6f842-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6f842-116">Application</span></span> | <span data-ttu-id="6f842-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f842-117">Directory.ReadWrite.All</span></span>|


## <a name="http-request"></a><span data-ttu-id="6f842-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6f842-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /organization/{organizationId}/activateService
```

## <a name="request-headers"></a><span data-ttu-id="6f842-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6f842-119">Request headers</span></span>
|<span data-ttu-id="6f842-120">Nome</span><span class="sxs-lookup"><span data-stu-id="6f842-120">Name</span></span>|<span data-ttu-id="6f842-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="6f842-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="6f842-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6f842-122">Authorization</span></span>|<span data-ttu-id="6f842-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6f842-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="6f842-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6f842-125">Content-Type</span></span>|<span data-ttu-id="6f842-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6f842-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6f842-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6f842-128">Request body</span></span>
<span data-ttu-id="6f842-129">No corpo da solicitação, fornece uma representação JSON do [objeto activateService.](../resources/activateService.md)</span><span class="sxs-lookup"><span data-stu-id="6f842-129">In the request body, supply a JSON representation of the [activateService](../resources/activateService.md) object.</span></span>
<span data-ttu-id="6f842-130">Você deve definir **o serviço** ou (**servicePlanId** _e_ **skuId**) para que essa ação seja válida.</span><span class="sxs-lookup"><span data-stu-id="6f842-130">You must define **service** or (**servicePlanId** _and_ **skuId**) for this action to be valid.</span></span>

| <span data-ttu-id="6f842-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6f842-131">Property</span></span>         | <span data-ttu-id="6f842-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="6f842-132">Type</span></span>         | <span data-ttu-id="6f842-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="6f842-133">Description</span></span>                           |
| ----------------- | ------------ | ------------------------------------- |
| <span data-ttu-id="6f842-134">service</span><span class="sxs-lookup"><span data-stu-id="6f842-134">service</span></span>| <span data-ttu-id="6f842-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6f842-135">String</span></span> | <span data-ttu-id="6f842-136">O nome do serviço a ser ativado.</span><span class="sxs-lookup"><span data-stu-id="6f842-136">The name of the service to activate.</span></span> |
| <span data-ttu-id="6f842-137">servicePlanId</span><span class="sxs-lookup"><span data-stu-id="6f842-137">servicePlanId</span></span> | <span data-ttu-id="6f842-138">Guid</span><span class="sxs-lookup"><span data-stu-id="6f842-138">Guid</span></span> | <span data-ttu-id="6f842-139">O identificador de plano do plano de serviço a ser ativado.</span><span class="sxs-lookup"><span data-stu-id="6f842-139">The plan identifier of the service plan to activate.</span></span> |
| <span data-ttu-id="6f842-140">skuId</span><span class="sxs-lookup"><span data-stu-id="6f842-140">skuId</span></span> | <span data-ttu-id="6f842-141">Guid</span><span class="sxs-lookup"><span data-stu-id="6f842-141">Guid</span></span> | <span data-ttu-id="6f842-142">O identificador SKU do plano de serviço.</span><span class="sxs-lookup"><span data-stu-id="6f842-142">The SKU identifier of the service plan.</span></span> |

## <a name="response"></a><span data-ttu-id="6f842-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="6f842-143">Response</span></span>

<span data-ttu-id="6f842-144">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="6f842-144">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="6f842-145">Exemplos</span><span class="sxs-lookup"><span data-stu-id="6f842-145">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6f842-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6f842-146">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "organization_activateservice"
}
-->
``` http
POST https://graph.microsoft.com/beta/organization/{:organizationId}/activateService
Content-Type: application/json

{
    "skuId": "6fd2c87f-b296-42f0-b197-1e91e994b900",
    "servicePlanId": "a23b959c-7ce8-4e57-9140-b90eb88a9e97"
}
```

### <a name="response"></a><span data-ttu-id="6f842-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="6f842-147">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```