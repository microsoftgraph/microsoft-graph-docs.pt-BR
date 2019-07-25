---
title: Atualizar governanceRoleSetting
description: Atualize as propriedades de governanceRoleSetting.
localization_priority: Normal
ms.openlocfilehash: fc2cb9864d65ca32ae62a32201b3821ab16264e8
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35859084"
---
# <a name="update-governancerolesetting"></a><span data-ttu-id="fc252-103">Atualizar governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="fc252-103">Update governanceRoleSetting</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fc252-104">Atualize as propriedades de [governanceRoleSetting](../resources/governancerolesetting.md).</span><span class="sxs-lookup"><span data-stu-id="fc252-104">Update the properties of [governanceRoleSetting](../resources/governancerolesetting.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="fc252-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="fc252-105">Permissions</span></span>
<span data-ttu-id="fc252-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fc252-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="fc252-108">**Observação:** Essa API também exige que o solicitante tenha pelo menos uma `Active` atribuição de função de`owner` administrador `user access administrator`(ou) no recurso.</span><span class="sxs-lookup"><span data-stu-id="fc252-108">**Note:** This API also requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

|<span data-ttu-id="fc252-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fc252-109">Permission type</span></span>      | <span data-ttu-id="fc252-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="fc252-110">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fc252-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fc252-111">Delegated (work or school account)</span></span> | <span data-ttu-id="fc252-112">PrivilegedAccess. ReadWrite. AzureResources</span><span class="sxs-lookup"><span data-stu-id="fc252-112">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="fc252-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fc252-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fc252-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fc252-114">Not supported.</span></span>    |
|<span data-ttu-id="fc252-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fc252-115">Application</span></span> | <span data-ttu-id="fc252-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fc252-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fc252-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fc252-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /privilegedAccess/azureResources/roleSettings/{id}
```
## <a name="request-headers"></a><span data-ttu-id="fc252-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fc252-118">Request headers</span></span>
| <span data-ttu-id="fc252-119">Nome</span><span class="sxs-lookup"><span data-stu-id="fc252-119">Name</span></span>       | <span data-ttu-id="fc252-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="fc252-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="fc252-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="fc252-121">Authorization</span></span>  | <span data-ttu-id="fc252-122">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="fc252-122">Bearer {code}</span></span>|
| <span data-ttu-id="fc252-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="fc252-123">Content-type</span></span>  | <span data-ttu-id="fc252-124">application/json</span><span class="sxs-lookup"><span data-stu-id="fc252-124">application/json</span></span>|


## <a name="request-body"></a><span data-ttu-id="fc252-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fc252-125">Request body</span></span>
<span data-ttu-id="fc252-126">No corpo da solicitação, forneça os valores para [governanceRuleSettings](../resources/governancerulesetting.md) que precisam ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="fc252-126">In the request body, supply the values for [governanceRuleSettings](../resources/governancerulesetting.md) that need to be updated.</span></span> 

| <span data-ttu-id="fc252-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fc252-127">Property</span></span>     | <span data-ttu-id="fc252-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="fc252-128">Type</span></span>   |<span data-ttu-id="fc252-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="fc252-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fc252-130">adminEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="fc252-130">adminEligibleSettings</span></span>|<span data-ttu-id="fc252-131">coleção [governanceRuleSetting](../resources/governancerulesetting.md)</span><span class="sxs-lookup"><span data-stu-id="fc252-131">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="fc252-132">As configurações de regra que são avaliadas quando um administrador tenta adicionar uma atribuição de função qualificada.</span><span class="sxs-lookup"><span data-stu-id="fc252-132">The rule settings that are evaluated when an administrator tries to add an eligible role assignment.</span></span>|
|<span data-ttu-id="fc252-133">adminMemberSettings</span><span class="sxs-lookup"><span data-stu-id="fc252-133">adminMemberSettings</span></span>|<span data-ttu-id="fc252-134">coleção [governanceRuleSetting](../resources/governancerulesetting.md)</span><span class="sxs-lookup"><span data-stu-id="fc252-134">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="fc252-135">As configurações de regra que são avaliadas quando um administrador tenta adicionar uma atribuição de função de membro direto.</span><span class="sxs-lookup"><span data-stu-id="fc252-135">The rule settings that are evaluated when an administrator tries to add a direct member role assignment.</span></span>|
|<span data-ttu-id="fc252-136">userEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="fc252-136">userEligibleSettings</span></span>|<span data-ttu-id="fc252-137">coleção [governanceRuleSetting](../resources/governancerulesetting.md)</span><span class="sxs-lookup"><span data-stu-id="fc252-137">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="fc252-138">As configurações de regra que são avaliadas quando um usuário tenta adicionar uma atribuição de função qualificada.</span><span class="sxs-lookup"><span data-stu-id="fc252-138">The rule settings that are evaluated when a user tries to add an eligible role assignment.</span></span> <span data-ttu-id="fc252-139">Isso não é suportado para `pimforazurerbac` o cenário por enquanto, e pode estar disponível nos cenários futuros.</span><span class="sxs-lookup"><span data-stu-id="fc252-139">This is not supported for `pimforazurerbac` scenario for now, and may be available in the future scenarios.</span></span>|
|<span data-ttu-id="fc252-140">userMemberSettings</span><span class="sxs-lookup"><span data-stu-id="fc252-140">userMemberSettings</span></span>|<span data-ttu-id="fc252-141">coleção [governanceRuleSetting](../resources/governancerulesetting.md)</span><span class="sxs-lookup"><span data-stu-id="fc252-141">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="fc252-142">As configurações de regra que são avaliadas quando um usuário tenta ativar sua atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="fc252-142">The rule settings that are evaluated when a user tries to activate his role assignment.</span></span>|

## <a name="response"></a><span data-ttu-id="fc252-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="fc252-143">Response</span></span>
<span data-ttu-id="fc252-p103">Se bem-sucedido, este método retorna um código de resposta `204 NoContent`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fc252-p103">If successful, this method returns a `204 NoContent` response code. It does not return anything in the response body.</span></span> 

### <a name="error-codes"></a><span data-ttu-id="fc252-146">Códigos de erro</span><span class="sxs-lookup"><span data-stu-id="fc252-146">Error codes</span></span>
<span data-ttu-id="fc252-147">Essa API retorna os códigos de erro HTTP padrão.</span><span class="sxs-lookup"><span data-stu-id="fc252-147">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="fc252-148">Além disso, ele retorna os seguintes códigos de erro personalizados.</span><span class="sxs-lookup"><span data-stu-id="fc252-148">In addition, it returns the following custom error codes.</span></span>

|<span data-ttu-id="fc252-149">Código de erro</span><span class="sxs-lookup"><span data-stu-id="fc252-149">Error code</span></span>     | <span data-ttu-id="fc252-150">Mensagem de erro</span><span class="sxs-lookup"><span data-stu-id="fc252-150">Error message</span></span>         | <span data-ttu-id="fc252-151">Detalhes</span><span class="sxs-lookup"><span data-stu-id="fc252-151">Details</span></span>             |
|:--------------| :---------------------|:--------------------|
| <span data-ttu-id="fc252-152">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="fc252-152">400 BadRequest</span></span>| <span data-ttu-id="fc252-153">RoleSettingNotFound</span><span class="sxs-lookup"><span data-stu-id="fc252-153">RoleSettingNotFound</span></span>   | <span data-ttu-id="fc252-154">O [governanceRoleSetting](../resources/governancerolesetting.md) não existe no sistema.</span><span class="sxs-lookup"><span data-stu-id="fc252-154">The [governanceRoleSetting](../resources/governancerolesetting.md) does not exist in system.</span></span>
| <span data-ttu-id="fc252-155">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="fc252-155">400 BadRequest</span></span>| <span data-ttu-id="fc252-156">InvalidRoleSetting</span><span class="sxs-lookup"><span data-stu-id="fc252-156">InvalidRoleSetting</span></span>    | <span data-ttu-id="fc252-157">Os valores de [governanceRuleSettings](../resources/governancerulesetting.md) fornecidos no corpo da solicitação não são válidos.</span><span class="sxs-lookup"><span data-stu-id="fc252-157">The [governanceRuleSettings](../resources/governancerulesetting.md) values provided in the request body are not valid.</span></span>

## <a name="example"></a><span data-ttu-id="fc252-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fc252-158">Example</span></span> 
<span data-ttu-id="fc252-159">Este exemplo atualiza a configuração de função para a função 3 personalizada na assinatura Wingtip Toys-prod.</span><span class="sxs-lookup"><span data-stu-id="fc252-159">This example updates the role setting for Custom Role 3 in the subscription Wingtip Toys - Prod.</span></span>
##### <a name="request"></a><span data-ttu-id="fc252-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fc252-160">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="fc252-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="fc252-161">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_governancerolesetting"
}-->
```http
PATCH https://graph.microsoft.com/beta/privilegedAccess/pimforazurerbac/roleSettings/5fb5aef8-1081-4b8e-bb16-9d5d0385bab5
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="fc252-162">C#</span><span class="sxs-lookup"><span data-stu-id="fc252-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-governancerolesetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fc252-163">Javascript</span><span class="sxs-lookup"><span data-stu-id="fc252-163">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-governancerolesetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fc252-164">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="fc252-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-governancerolesetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="fc252-165">Java</span><span class="sxs-lookup"><span data-stu-id="fc252-165">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-governancerolesetting-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="fc252-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="fc252-166">Response</span></span>
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
