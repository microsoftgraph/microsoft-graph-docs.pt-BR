---
title: Atualizar unifiedRoleManagementPolicyRule
description: Atualize as propriedades de um objeto unifiedRoleManagementPolicyRule.
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 05db197ef2fd4b54ea2036e42c06adc026f7746d
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/10/2021
ms.locfileid: "52299082"
---
# <a name="update-unifiedrolemanagementpolicyrule"></a><span data-ttu-id="47ffc-103">Atualizar unifiedRoleManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="47ffc-103">Update unifiedRoleManagementPolicyRule</span></span>
<span data-ttu-id="47ffc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="47ffc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="47ffc-105">Atualize as propriedades de [um objeto unifiedRoleManagementPolicyRule.](../resources/unifiedrolemanagementpolicyrule.md)</span><span class="sxs-lookup"><span data-stu-id="47ffc-105">Update the properties of an [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="47ffc-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="47ffc-106">Permissions</span></span>
<span data-ttu-id="47ffc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47ffc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47ffc-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="47ffc-109">Permission type</span></span>|<span data-ttu-id="47ffc-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="47ffc-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="47ffc-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="47ffc-111">Delegated (work or school account)</span></span>|<span data-ttu-id="47ffc-112">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="47ffc-112">PrivilegedAccess.ReadWrite.AzureAD</span></span>|
|<span data-ttu-id="47ffc-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="47ffc-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="47ffc-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="47ffc-114">Not supported</span></span>|
|<span data-ttu-id="47ffc-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="47ffc-115">Application</span></span>|<span data-ttu-id="47ffc-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="47ffc-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="47ffc-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="47ffc-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /policies/roleManagementPolicies/{unifiedRoleManagementPolicyId}/rules/{unifiedRoleManagementPolicyRuleId}
PATCH /policies/roleManagementPolicies/{unifiedRoleManagementPolicyId}/effectiveRules/{unifiedRoleManagementPolicyRuleId}
```

## <a name="request-headers"></a><span data-ttu-id="47ffc-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="47ffc-118">Request headers</span></span>
|<span data-ttu-id="47ffc-119">Nome</span><span class="sxs-lookup"><span data-stu-id="47ffc-119">Name</span></span>|<span data-ttu-id="47ffc-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="47ffc-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="47ffc-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="47ffc-121">Authorization</span></span>|<span data-ttu-id="47ffc-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="47ffc-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="47ffc-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="47ffc-124">Content-Type</span></span>|<span data-ttu-id="47ffc-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="47ffc-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="47ffc-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="47ffc-127">Request body</span></span>
<span data-ttu-id="47ffc-128">No corpo da solicitação, fornece uma representação JSON do [objeto unifiedRoleManagementPolicyRule.](../resources/unifiedrolemanagementpolicyrule.md)</span><span class="sxs-lookup"><span data-stu-id="47ffc-128">In the request body, supply a JSON representation of the [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) object.</span></span>

<span data-ttu-id="47ffc-129">A tabela a seguir mostra as propriedades que são necessárias ao atualizar [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md).</span><span class="sxs-lookup"><span data-stu-id="47ffc-129">The following table shows the properties that are required when you update the [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md).</span></span>

|<span data-ttu-id="47ffc-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="47ffc-130">Property</span></span>|<span data-ttu-id="47ffc-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="47ffc-131">Type</span></span>|<span data-ttu-id="47ffc-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="47ffc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47ffc-133">id</span><span class="sxs-lookup"><span data-stu-id="47ffc-133">id</span></span>|<span data-ttu-id="47ffc-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="47ffc-134">String</span></span>|<span data-ttu-id="47ffc-135">Identificador exclusivo da regra.</span><span class="sxs-lookup"><span data-stu-id="47ffc-135">Unique identifier for the rule.</span></span>|
|<span data-ttu-id="47ffc-136">destino</span><span class="sxs-lookup"><span data-stu-id="47ffc-136">target</span></span>|[<span data-ttu-id="47ffc-137">unifiedRoleManagementPolicyRuleTarget</span><span class="sxs-lookup"><span data-stu-id="47ffc-137">unifiedRoleManagementPolicyRuleTarget</span></span>](../resources/unifiedrolemanagementpolicyruletarget.md)|<span data-ttu-id="47ffc-138">O destino da regra de política.</span><span class="sxs-lookup"><span data-stu-id="47ffc-138">The target for the policy rule.</span></span>|



## <a name="response"></a><span data-ttu-id="47ffc-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="47ffc-139">Response</span></span>

<span data-ttu-id="47ffc-140">Se tiver êxito, este método retornará um código de resposta e um objeto `200 OK` [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="47ffc-140">If successful, this method returns a `200 OK` response code and an updated [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="47ffc-141">Exemplos</span><span class="sxs-lookup"><span data-stu-id="47ffc-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="47ffc-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="47ffc-142">Request</span></span>
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


### <a name="response"></a><span data-ttu-id="47ffc-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="47ffc-143">Response</span></span>
<span data-ttu-id="47ffc-144">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="47ffc-144">**Note:** The response object shown here might be shortened for readability.</span></span>
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
