---
title: Atualizar governanceRoleSetting
description: Atualize as propriedades de governanceRoleSetting.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 3ae917f9b92ee743173842b3ed9ccf2a2bea3edd
ms.sourcegitcommit: 21481acf54471ff17ab8043b3a96fcb1d2f863d7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/21/2020
ms.locfileid: "48634855"
---
# <a name="update-governancerolesetting"></a><span data-ttu-id="351c2-103">Atualizar governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="351c2-103">Update governanceRoleSetting</span></span>

<span data-ttu-id="351c2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="351c2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="351c2-105">Atualize as propriedades de [governanceRoleSetting](../resources/governancerolesetting.md).</span><span class="sxs-lookup"><span data-stu-id="351c2-105">Update the properties of [governanceRoleSetting](../resources/governancerolesetting.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="351c2-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="351c2-106">Permissions</span></span>
<span data-ttu-id="351c2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference#privileged-access-permissions).</span><span class="sxs-lookup"><span data-stu-id="351c2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference#privileged-access-permissions).</span></span>

><span data-ttu-id="351c2-109">**Observação:** Essa API também exige que o solicitante tenha pelo menos uma `Active` atribuição de função de administrador ( `owner` ou `user access administrator` ) no recurso.</span><span class="sxs-lookup"><span data-stu-id="351c2-109">**Note:** This API also requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

|<span data-ttu-id="351c2-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="351c2-110">Permission type</span></span>      | <span data-ttu-id="351c2-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="351c2-111">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="351c2-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="351c2-112">Delegated (work or school account)</span></span> | <span data-ttu-id="351c2-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="351c2-113">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="351c2-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="351c2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="351c2-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="351c2-115">Not supported.</span></span>    |
|<span data-ttu-id="351c2-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="351c2-116">Application</span></span> | <span data-ttu-id="351c2-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="351c2-117">Not supported.</span></span> |
### <a name="azure-resources"></a><span data-ttu-id="351c2-118">Recursos do Azure</span><span class="sxs-lookup"><span data-stu-id="351c2-118">Azure resources</span></span>

| <span data-ttu-id="351c2-119">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="351c2-119">Permission type</span></span> | <span data-ttu-id="351c2-120">Permissões</span><span class="sxs-lookup"><span data-stu-id="351c2-120">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="351c2-121">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="351c2-121">Delegated (work or school account)</span></span> | <span data-ttu-id="351c2-122">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="351c2-122">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="351c2-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="351c2-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="351c2-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="351c2-124">Not supported.</span></span> |
| <span data-ttu-id="351c2-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="351c2-125">Application</span></span> | <span data-ttu-id="351c2-126">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="351c2-126">Not supported.</span></span> |

### <a name="azure-ad"></a><span data-ttu-id="351c2-127">Azure AD</span><span class="sxs-lookup"><span data-stu-id="351c2-127">Azure AD</span></span>

| <span data-ttu-id="351c2-128">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="351c2-128">Permission type</span></span> | <span data-ttu-id="351c2-129">Permissões</span><span class="sxs-lookup"><span data-stu-id="351c2-129">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="351c2-130">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="351c2-130">Delegated (work or school account)</span></span> | <span data-ttu-id="351c2-131">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="351c2-131">PrivilegedAccess.ReadWrite.AzureAD</span></span> |
| <span data-ttu-id="351c2-132">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="351c2-132">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="351c2-133">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="351c2-133">Not supported.</span></span> |
| <span data-ttu-id="351c2-134">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="351c2-134">Application</span></span> | <span data-ttu-id="351c2-135">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="351c2-135">Not supported.</span></span> |

### <a name="groups"></a><span data-ttu-id="351c2-136">Grupos</span><span class="sxs-lookup"><span data-stu-id="351c2-136">Groups</span></span>

|<span data-ttu-id="351c2-137">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="351c2-137">Permission type</span></span> | <span data-ttu-id="351c2-138">Permissões</span><span class="sxs-lookup"><span data-stu-id="351c2-138">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="351c2-139">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="351c2-139">Delegated (work or school account)</span></span> | <span data-ttu-id="351c2-140">PrivilegedAccess. ReadWrite. AzureADGroups</span><span class="sxs-lookup"><span data-stu-id="351c2-140">PrivilegedAccess.ReadWrite.AzureADGroups</span></span> |
| <span data-ttu-id="351c2-141">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="351c2-141">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="351c2-142">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="351c2-142">Not supported.</span></span> |
| <span data-ttu-id="351c2-143">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="351c2-143">Application</span></span> | <span data-ttu-id="351c2-144">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="351c2-144">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="351c2-145">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="351c2-145">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /privilegedAccess/azureResources/roleSettings/{id}
```
## <a name="request-headers"></a><span data-ttu-id="351c2-146">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="351c2-146">Request headers</span></span>
| <span data-ttu-id="351c2-147">Nome</span><span class="sxs-lookup"><span data-stu-id="351c2-147">Name</span></span>       | <span data-ttu-id="351c2-148">Descrição</span><span class="sxs-lookup"><span data-stu-id="351c2-148">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="351c2-149">Autorização</span><span class="sxs-lookup"><span data-stu-id="351c2-149">Authorization</span></span>  | <span data-ttu-id="351c2-150">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="351c2-150">Bearer {token}</span></span>|
| <span data-ttu-id="351c2-151">Content-type</span><span class="sxs-lookup"><span data-stu-id="351c2-151">Content-type</span></span>  | <span data-ttu-id="351c2-152">application/json</span><span class="sxs-lookup"><span data-stu-id="351c2-152">application/json</span></span>|


## <a name="request-body"></a><span data-ttu-id="351c2-153">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="351c2-153">Request body</span></span>
<span data-ttu-id="351c2-154">No corpo da solicitação, forneça os valores para [governanceRuleSettings](../resources/governancerulesetting.md) que precisam ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="351c2-154">In the request body, supply the values for [governanceRuleSettings](../resources/governancerulesetting.md) that need to be updated.</span></span> 

| <span data-ttu-id="351c2-155">Propriedade</span><span class="sxs-lookup"><span data-stu-id="351c2-155">Property</span></span>     | <span data-ttu-id="351c2-156">Tipo</span><span class="sxs-lookup"><span data-stu-id="351c2-156">Type</span></span>   |<span data-ttu-id="351c2-157">Descrição</span><span class="sxs-lookup"><span data-stu-id="351c2-157">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="351c2-158">adminEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="351c2-158">adminEligibleSettings</span></span>|<span data-ttu-id="351c2-159">coleção [governanceRuleSetting](../resources/governancerulesetting.md)</span><span class="sxs-lookup"><span data-stu-id="351c2-159">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="351c2-160">As configurações de regra que são avaliadas quando um administrador tenta adicionar uma atribuição de função qualificada.</span><span class="sxs-lookup"><span data-stu-id="351c2-160">The rule settings that are evaluated when an administrator tries to add an eligible role assignment.</span></span>|
|<span data-ttu-id="351c2-161">adminMemberSettings</span><span class="sxs-lookup"><span data-stu-id="351c2-161">adminMemberSettings</span></span>|<span data-ttu-id="351c2-162">coleção [governanceRuleSetting](../resources/governancerulesetting.md)</span><span class="sxs-lookup"><span data-stu-id="351c2-162">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="351c2-163">As configurações de regra que são avaliadas quando um administrador tenta adicionar uma atribuição de função de membro direto.</span><span class="sxs-lookup"><span data-stu-id="351c2-163">The rule settings that are evaluated when an administrator tries to add a direct member role assignment.</span></span>|
|<span data-ttu-id="351c2-164">userEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="351c2-164">userEligibleSettings</span></span>|<span data-ttu-id="351c2-165">coleção [governanceRuleSetting](../resources/governancerulesetting.md)</span><span class="sxs-lookup"><span data-stu-id="351c2-165">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="351c2-166">As configurações de regra que são avaliadas quando um usuário tenta adicionar uma atribuição de função qualificada.</span><span class="sxs-lookup"><span data-stu-id="351c2-166">The rule settings that are evaluated when a user tries to add an eligible role assignment.</span></span> |
|<span data-ttu-id="351c2-167">userMemberSettings</span><span class="sxs-lookup"><span data-stu-id="351c2-167">userMemberSettings</span></span>|<span data-ttu-id="351c2-168">coleção [governanceRuleSetting](../resources/governancerulesetting.md)</span><span class="sxs-lookup"><span data-stu-id="351c2-168">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="351c2-169">As configurações de regra que são avaliadas quando um usuário tenta ativar sua atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="351c2-169">The rule settings that are evaluated when a user tries to activate his role assignment.</span></span>|

## <a name="response"></a><span data-ttu-id="351c2-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="351c2-170">Response</span></span>
<span data-ttu-id="351c2-p102">Se bem-sucedido, este método retorna um código de resposta `204 NoContent`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="351c2-p102">If successful, this method returns a `204 NoContent` response code. It does not return anything in the response body.</span></span> 

### <a name="error-codes"></a><span data-ttu-id="351c2-173">Códigos de erro</span><span class="sxs-lookup"><span data-stu-id="351c2-173">Error codes</span></span>
<span data-ttu-id="351c2-174">Essa API retorna os códigos de erro HTTP padrão.</span><span class="sxs-lookup"><span data-stu-id="351c2-174">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="351c2-175">Além disso, ele retorna os seguintes códigos de erro personalizados.</span><span class="sxs-lookup"><span data-stu-id="351c2-175">In addition, it returns the following custom error codes.</span></span>

|<span data-ttu-id="351c2-176">Código de erro</span><span class="sxs-lookup"><span data-stu-id="351c2-176">Error code</span></span>     | <span data-ttu-id="351c2-177">Mensagem de erro</span><span class="sxs-lookup"><span data-stu-id="351c2-177">Error message</span></span>         | <span data-ttu-id="351c2-178">Detalhes</span><span class="sxs-lookup"><span data-stu-id="351c2-178">Details</span></span>             |
|:--------------| :---------------------|:--------------------|
| <span data-ttu-id="351c2-179">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="351c2-179">400 BadRequest</span></span>| <span data-ttu-id="351c2-180">RoleSettingNotFound</span><span class="sxs-lookup"><span data-stu-id="351c2-180">RoleSettingNotFound</span></span>   | <span data-ttu-id="351c2-181">O [governanceRoleSetting](../resources/governancerolesetting.md) não existe no sistema.</span><span class="sxs-lookup"><span data-stu-id="351c2-181">The [governanceRoleSetting](../resources/governancerolesetting.md) does not exist in system.</span></span>
| <span data-ttu-id="351c2-182">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="351c2-182">400 BadRequest</span></span>| <span data-ttu-id="351c2-183">InvalidRoleSetting</span><span class="sxs-lookup"><span data-stu-id="351c2-183">InvalidRoleSetting</span></span>    | <span data-ttu-id="351c2-184">Os valores de [governanceRuleSettings](../resources/governancerulesetting.md) fornecidos no corpo da solicitação não são válidos.</span><span class="sxs-lookup"><span data-stu-id="351c2-184">The [governanceRuleSettings](../resources/governancerulesetting.md) values provided in the request body are not valid.</span></span>

## <a name="example"></a><span data-ttu-id="351c2-185">Exemplo</span><span class="sxs-lookup"><span data-stu-id="351c2-185">Example</span></span> 
<span data-ttu-id="351c2-186">Este exemplo atualiza a configuração de função para a função 3 personalizada na assinatura Wingtip Toys-prod.</span><span class="sxs-lookup"><span data-stu-id="351c2-186">This example updates the role setting for Custom Role 3 in the subscription Wingtip Toys - Prod.</span></span>
##### <a name="request"></a><span data-ttu-id="351c2-187">Solicitação</span><span class="sxs-lookup"><span data-stu-id="351c2-187">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="351c2-188">HTTP</span><span class="sxs-lookup"><span data-stu-id="351c2-188">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_governancerolesetting"
}-->
```http
PATCH https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleSettings/5fb5aef8-1081-4b8e-bb16-9d5d0385bab5
Content-type: application/json
Content-length: 350

{
   "adminEligibleSettings":[
      {
         "ruleIdentifier":"ExpirationRule",
         "setting":"{\"permanentAssignment\":false,\"maximumGrantPeriodInMinutes\":129600}"
      }
   ]
}
```
# <a name="c"></a>[<span data-ttu-id="351c2-189">C#</span><span class="sxs-lookup"><span data-stu-id="351c2-189">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-governancerolesetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="351c2-190">JavaScript</span><span class="sxs-lookup"><span data-stu-id="351c2-190">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-governancerolesetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="351c2-191">Objective-C</span><span class="sxs-lookup"><span data-stu-id="351c2-191">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-governancerolesetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="351c2-192">Resposta</span><span class="sxs-lookup"><span data-stu-id="351c2-192">Response</span></span>
<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update governanceRoleSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


