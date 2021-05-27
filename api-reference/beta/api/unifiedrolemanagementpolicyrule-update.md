---
title: Atualizar unifiedRoleManagementPolicyRule
description: Atualize as propriedades de um objeto unifiedRoleManagementPolicyRule.
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 5c5e8fe49f4d88d07c5627b55db6fd0f5e3839e8
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/27/2021
ms.locfileid: "52682282"
---
# <a name="update-unifiedrolemanagementpolicyrule"></a><span data-ttu-id="49be7-103">Atualizar unifiedRoleManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="49be7-103">Update unifiedRoleManagementPolicyRule</span></span>
<span data-ttu-id="49be7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="49be7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="49be7-105">Atualize as propriedades de [um objeto unifiedRoleManagementPolicyRule.](../resources/unifiedrolemanagementpolicyrule.md)</span><span class="sxs-lookup"><span data-stu-id="49be7-105">Update the properties of an [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="49be7-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="49be7-106">Permissions</span></span>
<span data-ttu-id="49be7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49be7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49be7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="49be7-109">Permission type</span></span>|<span data-ttu-id="49be7-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="49be7-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="49be7-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="49be7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="49be7-112">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="49be7-112">PrivilegedAccess.ReadWrite.AzureAD</span></span>|
|<span data-ttu-id="49be7-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="49be7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="49be7-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="49be7-114">Not supported</span></span>|
|<span data-ttu-id="49be7-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="49be7-115">Application</span></span>|<span data-ttu-id="49be7-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="49be7-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="49be7-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="49be7-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /policies/roleManagementPolicies/{unifiedRoleManagementPolicyId}/rules/{unifiedRoleManagementPolicyRuleId}
PATCH /policies/roleManagementPolicies/{unifiedRoleManagementPolicyId}/effectiveRules/{unifiedRoleManagementPolicyRuleId}
```

## <a name="request-headers"></a><span data-ttu-id="49be7-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="49be7-118">Request headers</span></span>
|<span data-ttu-id="49be7-119">Nome</span><span class="sxs-lookup"><span data-stu-id="49be7-119">Name</span></span>|<span data-ttu-id="49be7-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="49be7-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="49be7-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="49be7-121">Authorization</span></span>|<span data-ttu-id="49be7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="49be7-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="49be7-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="49be7-124">Content-Type</span></span>|<span data-ttu-id="49be7-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="49be7-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="49be7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="49be7-127">Request body</span></span>
<span data-ttu-id="49be7-128">No corpo da solicitação, fornece uma representação JSON do [objeto unifiedRoleManagementPolicyRule.](../resources/unifiedrolemanagementpolicyrule.md)</span><span class="sxs-lookup"><span data-stu-id="49be7-128">In the request body, supply a JSON representation of the [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) object.</span></span>

<span data-ttu-id="49be7-129">A tabela a seguir mostra as propriedades que são necessárias ao atualizar [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md).</span><span class="sxs-lookup"><span data-stu-id="49be7-129">The following table shows the properties that are required when you update the [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md).</span></span>

|<span data-ttu-id="49be7-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="49be7-130">Property</span></span>|<span data-ttu-id="49be7-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="49be7-131">Type</span></span>|<span data-ttu-id="49be7-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="49be7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49be7-133">id</span><span class="sxs-lookup"><span data-stu-id="49be7-133">id</span></span>|<span data-ttu-id="49be7-134">String</span><span class="sxs-lookup"><span data-stu-id="49be7-134">String</span></span>|<span data-ttu-id="49be7-135">Identificador exclusivo da regra.</span><span class="sxs-lookup"><span data-stu-id="49be7-135">Unique identifier for the rule.</span></span>|
|<span data-ttu-id="49be7-136">destino</span><span class="sxs-lookup"><span data-stu-id="49be7-136">target</span></span>|[<span data-ttu-id="49be7-137">unifiedRoleManagementPolicyRuleTarget</span><span class="sxs-lookup"><span data-stu-id="49be7-137">unifiedRoleManagementPolicyRuleTarget</span></span>](../resources/unifiedrolemanagementpolicyruletarget.md)|<span data-ttu-id="49be7-138">O destino da regra de política.</span><span class="sxs-lookup"><span data-stu-id="49be7-138">The target for the policy rule.</span></span>|



## <a name="response"></a><span data-ttu-id="49be7-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="49be7-139">Response</span></span>

<span data-ttu-id="49be7-140">Se tiver êxito, este método retornará um código de resposta e um objeto `200 OK` [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="49be7-140">If successful, this method returns a `200 OK` response code and an updated [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="49be7-141">Exemplos</span><span class="sxs-lookup"><span data-stu-id="49be7-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="49be7-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="49be7-142">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="49be7-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="49be7-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_unifiedrolemanagementpolicyrule"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/policies/roleManagementPolicies/{unifiedRoleManagementPolicyId}/rules/{unifiedRoleManagementPolicyRuleId}
Content-Type: application/json
Content-length: 170

{
  "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyRule",
  "target": {
    "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyRuleTarget"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="49be7-144">C#</span><span class="sxs-lookup"><span data-stu-id="49be7-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-unifiedrolemanagementpolicyrule-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="49be7-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="49be7-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-unifiedrolemanagementpolicyrule-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="49be7-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="49be7-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-unifiedrolemanagementpolicyrule-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="49be7-147">Java</span><span class="sxs-lookup"><span data-stu-id="49be7-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-unifiedrolemanagementpolicyrule-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="49be7-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="49be7-148">Response</span></span>
<span data-ttu-id="49be7-149">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="49be7-149">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyRule"
}
-->
```http
HTTP/1.1 204 OK

```
<!--
{
  "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyRule",
  "id": "ba9cc2d6-c2d6-ba9c-d6c2-9cbad6c29cba",
  "target": {
    "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyRuleTarget"
  }
}
```
-->
