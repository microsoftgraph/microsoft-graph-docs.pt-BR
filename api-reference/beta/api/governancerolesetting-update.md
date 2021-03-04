---
title: Atualizar governançaRoleSetting
description: Atualize as propriedades de governanceRoleSetting.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 2c4392529d64683a183002b9f0b302495f8042e5
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50435781"
---
# <a name="update-governancerolesetting"></a><span data-ttu-id="f0383-103">Atualizar governançaRoleSetting</span><span class="sxs-lookup"><span data-stu-id="f0383-103">Update governanceRoleSetting</span></span>

<span data-ttu-id="f0383-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f0383-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f0383-105">Atualize as propriedades [de governanceRoleSetting](../resources/governancerolesetting.md).</span><span class="sxs-lookup"><span data-stu-id="f0383-105">Update the properties of [governanceRoleSetting](../resources/governancerolesetting.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f0383-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f0383-106">Permissions</span></span>
<span data-ttu-id="f0383-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference#privileged-access-permissions).</span><span class="sxs-lookup"><span data-stu-id="f0383-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference#privileged-access-permissions).</span></span>

><span data-ttu-id="f0383-109">**Observação:** Essa API também exige que o solicitante tenha pelo menos uma atribuição de função de `Active` administrador ( ou ) no `owner` `user access administrator` recurso.</span><span class="sxs-lookup"><span data-stu-id="f0383-109">**Note:** This API also requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

|<span data-ttu-id="f0383-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f0383-110">Permission type</span></span>      | <span data-ttu-id="f0383-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="f0383-111">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f0383-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f0383-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f0383-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="f0383-113">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="f0383-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f0383-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f0383-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f0383-115">Not supported.</span></span>    |
|<span data-ttu-id="f0383-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f0383-116">Application</span></span> | <span data-ttu-id="f0383-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f0383-117">Not supported.</span></span> |
### <a name="azure-resources"></a><span data-ttu-id="f0383-118">Recursos do Azure</span><span class="sxs-lookup"><span data-stu-id="f0383-118">Azure resources</span></span>

| <span data-ttu-id="f0383-119">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f0383-119">Permission type</span></span> | <span data-ttu-id="f0383-120">Permissões</span><span class="sxs-lookup"><span data-stu-id="f0383-120">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="f0383-121">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f0383-121">Delegated (work or school account)</span></span> | <span data-ttu-id="f0383-122">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="f0383-122">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="f0383-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f0383-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f0383-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f0383-124">Not supported.</span></span> |
| <span data-ttu-id="f0383-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f0383-125">Application</span></span> | <span data-ttu-id="f0383-126">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f0383-126">Not supported.</span></span> |

### <a name="azure-ad"></a><span data-ttu-id="f0383-127">Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="f0383-127">Azure AD</span></span>

| <span data-ttu-id="f0383-128">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f0383-128">Permission type</span></span> | <span data-ttu-id="f0383-129">Permissões</span><span class="sxs-lookup"><span data-stu-id="f0383-129">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="f0383-130">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f0383-130">Delegated (work or school account)</span></span> | <span data-ttu-id="f0383-131">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="f0383-131">PrivilegedAccess.ReadWrite.AzureAD</span></span> |
| <span data-ttu-id="f0383-132">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f0383-132">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f0383-133">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f0383-133">Not supported.</span></span> |
| <span data-ttu-id="f0383-134">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f0383-134">Application</span></span> | <span data-ttu-id="f0383-135">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f0383-135">Not supported.</span></span> |

### <a name="groups"></a><span data-ttu-id="f0383-136">Grupos</span><span class="sxs-lookup"><span data-stu-id="f0383-136">Groups</span></span>

|<span data-ttu-id="f0383-137">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f0383-137">Permission type</span></span> | <span data-ttu-id="f0383-138">Permissões</span><span class="sxs-lookup"><span data-stu-id="f0383-138">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="f0383-139">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f0383-139">Delegated (work or school account)</span></span> | <span data-ttu-id="f0383-140">PrivilegedAccess.ReadWrite.AzureADGroups</span><span class="sxs-lookup"><span data-stu-id="f0383-140">PrivilegedAccess.ReadWrite.AzureADGroups</span></span> |
| <span data-ttu-id="f0383-141">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f0383-141">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f0383-142">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f0383-142">Not supported.</span></span> |
| <span data-ttu-id="f0383-143">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f0383-143">Application</span></span> | <span data-ttu-id="f0383-144">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f0383-144">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f0383-145">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f0383-145">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /privilegedAccess/azureResources/roleSettings/{id}
```
## <a name="request-headers"></a><span data-ttu-id="f0383-146">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f0383-146">Request headers</span></span>
| <span data-ttu-id="f0383-147">Nome</span><span class="sxs-lookup"><span data-stu-id="f0383-147">Name</span></span>       | <span data-ttu-id="f0383-148">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0383-148">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="f0383-149">Autorização</span><span class="sxs-lookup"><span data-stu-id="f0383-149">Authorization</span></span>  | <span data-ttu-id="f0383-150">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="f0383-150">Bearer {token}</span></span>|
| <span data-ttu-id="f0383-151">Content-type</span><span class="sxs-lookup"><span data-stu-id="f0383-151">Content-type</span></span>  | <span data-ttu-id="f0383-152">application/json</span><span class="sxs-lookup"><span data-stu-id="f0383-152">application/json</span></span>|


## <a name="request-body"></a><span data-ttu-id="f0383-153">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f0383-153">Request body</span></span>
<span data-ttu-id="f0383-154">No corpo da solicitação, fornece os valores [para governanceRuleSettings](../resources/governancerulesetting.md) que precisam ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="f0383-154">In the request body, supply the values for [governanceRuleSettings](../resources/governancerulesetting.md) that need to be updated.</span></span> 

| <span data-ttu-id="f0383-155">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f0383-155">Property</span></span>     | <span data-ttu-id="f0383-156">Tipo</span><span class="sxs-lookup"><span data-stu-id="f0383-156">Type</span></span>   |<span data-ttu-id="f0383-157">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0383-157">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f0383-158">adminEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="f0383-158">adminEligibleSettings</span></span>|<span data-ttu-id="f0383-159">[Coleção governanceRuleSetting](../resources/governancerulesetting.md)</span><span class="sxs-lookup"><span data-stu-id="f0383-159">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="f0383-160">As configurações de regra avaliadas quando um administrador tenta adicionar uma atribuição de função qualificada.</span><span class="sxs-lookup"><span data-stu-id="f0383-160">The rule settings that are evaluated when an administrator tries to add an eligible role assignment.</span></span>|
|<span data-ttu-id="f0383-161">adminMemberSettings</span><span class="sxs-lookup"><span data-stu-id="f0383-161">adminMemberSettings</span></span>|<span data-ttu-id="f0383-162">[Coleção governanceRuleSetting](../resources/governancerulesetting.md)</span><span class="sxs-lookup"><span data-stu-id="f0383-162">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="f0383-163">As configurações de regra avaliadas quando um administrador tenta adicionar uma atribuição de função de membro direto.</span><span class="sxs-lookup"><span data-stu-id="f0383-163">The rule settings that are evaluated when an administrator tries to add a direct member role assignment.</span></span>|
|<span data-ttu-id="f0383-164">userEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="f0383-164">userEligibleSettings</span></span>|<span data-ttu-id="f0383-165">[Coleção governanceRuleSetting](../resources/governancerulesetting.md)</span><span class="sxs-lookup"><span data-stu-id="f0383-165">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="f0383-166">As configurações de regra avaliadas quando um usuário tenta adicionar uma atribuição de função qualificada.</span><span class="sxs-lookup"><span data-stu-id="f0383-166">The rule settings that are evaluated when a user tries to add an eligible role assignment.</span></span> |
|<span data-ttu-id="f0383-167">userMemberSettings</span><span class="sxs-lookup"><span data-stu-id="f0383-167">userMemberSettings</span></span>|<span data-ttu-id="f0383-168">[Coleção governanceRuleSetting](../resources/governancerulesetting.md)</span><span class="sxs-lookup"><span data-stu-id="f0383-168">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="f0383-169">As configurações de regra avaliadas quando um usuário tenta ativar sua atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="f0383-169">The rule settings that are evaluated when a user tries to activate his role assignment.</span></span>|

## <a name="response"></a><span data-ttu-id="f0383-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="f0383-170">Response</span></span>
<span data-ttu-id="f0383-p102">Se bem-sucedido, este método retorna um código de resposta `204 NoContent`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f0383-p102">If successful, this method returns a `204 NoContent` response code. It does not return anything in the response body.</span></span> 

### <a name="error-codes"></a><span data-ttu-id="f0383-173">Códigos de erro</span><span class="sxs-lookup"><span data-stu-id="f0383-173">Error codes</span></span>
<span data-ttu-id="f0383-174">Esta API retorna os códigos de erro HTTP padrão.</span><span class="sxs-lookup"><span data-stu-id="f0383-174">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="f0383-175">Além disso, ele retorna os seguintes códigos de erro personalizados.</span><span class="sxs-lookup"><span data-stu-id="f0383-175">In addition, it returns the following custom error codes.</span></span>

|<span data-ttu-id="f0383-176">Código de erro</span><span class="sxs-lookup"><span data-stu-id="f0383-176">Error code</span></span>     | <span data-ttu-id="f0383-177">Mensagem de erro</span><span class="sxs-lookup"><span data-stu-id="f0383-177">Error message</span></span>         | <span data-ttu-id="f0383-178">Detalhes</span><span class="sxs-lookup"><span data-stu-id="f0383-178">Details</span></span>             |
|:--------------| :---------------------|:--------------------|
| <span data-ttu-id="f0383-179">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="f0383-179">400 BadRequest</span></span>| <span data-ttu-id="f0383-180">RoleSettingNotFound</span><span class="sxs-lookup"><span data-stu-id="f0383-180">RoleSettingNotFound</span></span>   | <span data-ttu-id="f0383-181">O [governanceRoleSetting](../resources/governancerolesetting.md) não existe no sistema.</span><span class="sxs-lookup"><span data-stu-id="f0383-181">The [governanceRoleSetting](../resources/governancerolesetting.md) does not exist in system.</span></span>
| <span data-ttu-id="f0383-182">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="f0383-182">400 BadRequest</span></span>| <span data-ttu-id="f0383-183">InvalidRoleSetting</span><span class="sxs-lookup"><span data-stu-id="f0383-183">InvalidRoleSetting</span></span>    | <span data-ttu-id="f0383-184">Os [valores governanceRuleSettings fornecidos](../resources/governancerulesetting.md) no corpo da solicitação não são válidos.</span><span class="sxs-lookup"><span data-stu-id="f0383-184">The [governanceRuleSettings](../resources/governancerulesetting.md) values provided in the request body are not valid.</span></span>

## <a name="example"></a><span data-ttu-id="f0383-185">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f0383-185">Example</span></span> 
<span data-ttu-id="f0383-186">Este exemplo atualiza a configuração de função para Função Personalizada 3 na assinatura Wingtip Toys - Prod.</span><span class="sxs-lookup"><span data-stu-id="f0383-186">This example updates the role setting for Custom Role 3 in the subscription Wingtip Toys - Prod.</span></span>
##### <a name="request"></a><span data-ttu-id="f0383-187">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f0383-187">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="f0383-188">HTTP</span><span class="sxs-lookup"><span data-stu-id="f0383-188">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="f0383-189">C#</span><span class="sxs-lookup"><span data-stu-id="f0383-189">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-governancerolesetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f0383-190">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f0383-190">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-governancerolesetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f0383-191">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f0383-191">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-governancerolesetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f0383-192">Java</span><span class="sxs-lookup"><span data-stu-id="f0383-192">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-governancerolesetting-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f0383-193">Resposta</span><span class="sxs-lookup"><span data-stu-id="f0383-193">Response</span></span>
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


