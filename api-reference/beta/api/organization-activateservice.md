---
title: 'organization: activateService'
description: Ativa um serviço para uma organização.
author: dkershaw10
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: c65d864fcfcabab5616113528f3e347238828bc5
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53207659"
---
# <a name="organization-activateservice"></a><span data-ttu-id="bf951-103">organization: activateService</span><span class="sxs-lookup"><span data-stu-id="bf951-103">organization: activateService</span></span>

<span data-ttu-id="bf951-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bf951-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bf951-105">Ative um serviço para uma organização.</span><span class="sxs-lookup"><span data-stu-id="bf951-105">Activate a service for an organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="bf951-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="bf951-106">Permissions</span></span>
<span data-ttu-id="bf951-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bf951-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="bf951-109">Para ativar um serviço para uma organização, o  solicitante precisa ter a função administrador da empresa com as seguintes permissões.</span><span class="sxs-lookup"><span data-stu-id="bf951-109">In order to activate a service for an organization the requestor needs to have the _Company Administrator_ role with the following permissions.</span></span>

|<span data-ttu-id="bf951-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bf951-110">Permission type</span></span>|<span data-ttu-id="bf951-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bf951-111">Permissions (from least to most privileged)</span></span>|
| :--- | :--- |
| <span data-ttu-id="bf951-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bf951-112">Delegated (work or school account)</span></span> | <span data-ttu-id="bf951-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf951-113">Directory.ReadWrite.All</span></span>|
| <span data-ttu-id="bf951-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bf951-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bf951-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bf951-115">Not Supported.</span></span> |
| <span data-ttu-id="bf951-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bf951-116">Application</span></span> | <span data-ttu-id="bf951-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf951-117">Directory.ReadWrite.All</span></span>|


## <a name="http-request"></a><span data-ttu-id="bf951-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bf951-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /organization/{organizationId}/activateService
```

## <a name="request-headers"></a><span data-ttu-id="bf951-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bf951-119">Request headers</span></span>
|<span data-ttu-id="bf951-120">Nome</span><span class="sxs-lookup"><span data-stu-id="bf951-120">Name</span></span>|<span data-ttu-id="bf951-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="bf951-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="bf951-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="bf951-122">Authorization</span></span>|<span data-ttu-id="bf951-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bf951-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="bf951-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bf951-125">Content-Type</span></span>|<span data-ttu-id="bf951-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bf951-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bf951-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bf951-128">Request body</span></span>
<span data-ttu-id="bf951-129">No corpo da solicitação, fornece uma representação JSON do [objeto activateService.](../resources/activateService.md)</span><span class="sxs-lookup"><span data-stu-id="bf951-129">In the request body, supply a JSON representation of the [activateService](../resources/activateService.md) object.</span></span>
<span data-ttu-id="bf951-130">Você deve definir **o serviço** ou (**servicePlanId** _e_ **skuId**) para que essa ação seja válida.</span><span class="sxs-lookup"><span data-stu-id="bf951-130">You must define **service** or (**servicePlanId** _and_ **skuId**) for this action to be valid.</span></span>

| <span data-ttu-id="bf951-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bf951-131">Property</span></span>         | <span data-ttu-id="bf951-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="bf951-132">Type</span></span>         | <span data-ttu-id="bf951-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="bf951-133">Description</span></span>                           |
| ----------------- | ------------ | ------------------------------------- |
| <span data-ttu-id="bf951-134">service</span><span class="sxs-lookup"><span data-stu-id="bf951-134">service</span></span>| <span data-ttu-id="bf951-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bf951-135">String</span></span> | <span data-ttu-id="bf951-136">O nome do serviço a ser ativado.</span><span class="sxs-lookup"><span data-stu-id="bf951-136">The name of the service to activate.</span></span> |
| <span data-ttu-id="bf951-137">servicePlanId</span><span class="sxs-lookup"><span data-stu-id="bf951-137">servicePlanId</span></span> | <span data-ttu-id="bf951-138">Guid</span><span class="sxs-lookup"><span data-stu-id="bf951-138">Guid</span></span> | <span data-ttu-id="bf951-139">O identificador de plano do plano de serviço a ser ativado.</span><span class="sxs-lookup"><span data-stu-id="bf951-139">The plan identifier of the service plan to activate.</span></span> |
| <span data-ttu-id="bf951-140">skuId</span><span class="sxs-lookup"><span data-stu-id="bf951-140">skuId</span></span> | <span data-ttu-id="bf951-141">Guid</span><span class="sxs-lookup"><span data-stu-id="bf951-141">Guid</span></span> | <span data-ttu-id="bf951-142">O identificador SKU do plano de serviço.</span><span class="sxs-lookup"><span data-stu-id="bf951-142">The SKU identifier of the service plan.</span></span> |

## <a name="response"></a><span data-ttu-id="bf951-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="bf951-143">Response</span></span>

<span data-ttu-id="bf951-144">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="bf951-144">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="bf951-145">Exemplos</span><span class="sxs-lookup"><span data-stu-id="bf951-145">Examples</span></span>

### <a name="request"></a><span data-ttu-id="bf951-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bf951-146">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="bf951-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="bf951-147">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="bf951-148">C#</span><span class="sxs-lookup"><span data-stu-id="bf951-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/organization-activateservice-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bf951-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bf951-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/organization-activateservice-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bf951-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bf951-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/organization-activateservice-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bf951-151">Java</span><span class="sxs-lookup"><span data-stu-id="bf951-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/organization-activateservice-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="bf951-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="bf951-152">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
