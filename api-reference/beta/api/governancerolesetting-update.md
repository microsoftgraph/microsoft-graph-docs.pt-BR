---
title: Atualizar governanceRoleSetting
description: Atualize as propriedades de governanceRoleSetting.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: e8f18cae950276979330d0f4830acbd2eb4492ab
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/10/2020
ms.locfileid: "43215795"
---
# <a name="update-governancerolesetting"></a><span data-ttu-id="d7126-103">Atualizar governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="d7126-103">Update governanceRoleSetting</span></span>

<span data-ttu-id="d7126-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d7126-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d7126-105">Atualize as propriedades de [governanceRoleSetting](../resources/governancerolesetting.md).</span><span class="sxs-lookup"><span data-stu-id="d7126-105">Update the properties of [governanceRoleSetting](../resources/governancerolesetting.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d7126-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d7126-106">Permissions</span></span>
<span data-ttu-id="d7126-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d7126-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="d7126-109">**Observação:** Essa API também exige que o solicitante tenha pelo menos uma `Active` atribuição de função de`owner` administrador `user access administrator`(ou) no recurso.</span><span class="sxs-lookup"><span data-stu-id="d7126-109">**Note:** This API also requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

|<span data-ttu-id="d7126-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d7126-110">Permission type</span></span>      | <span data-ttu-id="d7126-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="d7126-111">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d7126-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d7126-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d7126-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="d7126-113">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="d7126-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d7126-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d7126-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d7126-115">Not supported.</span></span>    |
|<span data-ttu-id="d7126-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d7126-116">Application</span></span> | <span data-ttu-id="d7126-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d7126-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d7126-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d7126-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /privilegedAccess/azureResources/roleSettings/{id}
```
## <a name="request-headers"></a><span data-ttu-id="d7126-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d7126-119">Request headers</span></span>
| <span data-ttu-id="d7126-120">Nome</span><span class="sxs-lookup"><span data-stu-id="d7126-120">Name</span></span>       | <span data-ttu-id="d7126-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="d7126-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="d7126-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d7126-122">Authorization</span></span>  | <span data-ttu-id="d7126-123">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="d7126-123">Bearer {token}</span></span>|
| <span data-ttu-id="d7126-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="d7126-124">Content-type</span></span>  | <span data-ttu-id="d7126-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d7126-125">application/json</span></span>|


## <a name="request-body"></a><span data-ttu-id="d7126-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d7126-126">Request body</span></span>
<span data-ttu-id="d7126-127">No corpo da solicitação, forneça os valores para [governanceRuleSettings](../resources/governancerulesetting.md) que precisam ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="d7126-127">In the request body, supply the values for [governanceRuleSettings](../resources/governancerulesetting.md) that need to be updated.</span></span> 

| <span data-ttu-id="d7126-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d7126-128">Property</span></span>     | <span data-ttu-id="d7126-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="d7126-129">Type</span></span>   |<span data-ttu-id="d7126-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="d7126-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d7126-131">adminEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="d7126-131">adminEligibleSettings</span></span>|<span data-ttu-id="d7126-132">coleção [governanceRuleSetting](../resources/governancerulesetting.md)</span><span class="sxs-lookup"><span data-stu-id="d7126-132">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="d7126-133">As configurações de regra que são avaliadas quando um administrador tenta adicionar uma atribuição de função qualificada.</span><span class="sxs-lookup"><span data-stu-id="d7126-133">The rule settings that are evaluated when an administrator tries to add an eligible role assignment.</span></span>|
|<span data-ttu-id="d7126-134">adminMemberSettings</span><span class="sxs-lookup"><span data-stu-id="d7126-134">adminMemberSettings</span></span>|<span data-ttu-id="d7126-135">coleção [governanceRuleSetting](../resources/governancerulesetting.md)</span><span class="sxs-lookup"><span data-stu-id="d7126-135">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="d7126-136">As configurações de regra que são avaliadas quando um administrador tenta adicionar uma atribuição de função de membro direto.</span><span class="sxs-lookup"><span data-stu-id="d7126-136">The rule settings that are evaluated when an administrator tries to add a direct member role assignment.</span></span>|
|<span data-ttu-id="d7126-137">userEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="d7126-137">userEligibleSettings</span></span>|<span data-ttu-id="d7126-138">coleção [governanceRuleSetting](../resources/governancerulesetting.md)</span><span class="sxs-lookup"><span data-stu-id="d7126-138">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="d7126-139">As configurações de regra que são avaliadas quando um usuário tenta adicionar uma atribuição de função qualificada.</span><span class="sxs-lookup"><span data-stu-id="d7126-139">The rule settings that are evaluated when a user tries to add an eligible role assignment.</span></span> |
|<span data-ttu-id="d7126-140">userMemberSettings</span><span class="sxs-lookup"><span data-stu-id="d7126-140">userMemberSettings</span></span>|<span data-ttu-id="d7126-141">coleção [governanceRuleSetting](../resources/governancerulesetting.md)</span><span class="sxs-lookup"><span data-stu-id="d7126-141">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="d7126-142">As configurações de regra que são avaliadas quando um usuário tenta ativar sua atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="d7126-142">The rule settings that are evaluated when a user tries to activate his role assignment.</span></span>|

## <a name="response"></a><span data-ttu-id="d7126-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="d7126-143">Response</span></span>
<span data-ttu-id="d7126-p102">Se bem-sucedido, este método retorna um código de resposta `204 NoContent`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d7126-p102">If successful, this method returns a `204 NoContent` response code. It does not return anything in the response body.</span></span> 

### <a name="error-codes"></a><span data-ttu-id="d7126-146">Códigos de erro</span><span class="sxs-lookup"><span data-stu-id="d7126-146">Error codes</span></span>
<span data-ttu-id="d7126-147">Essa API retorna os códigos de erro HTTP padrão.</span><span class="sxs-lookup"><span data-stu-id="d7126-147">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="d7126-148">Além disso, ele retorna os seguintes códigos de erro personalizados.</span><span class="sxs-lookup"><span data-stu-id="d7126-148">In addition, it returns the following custom error codes.</span></span>

|<span data-ttu-id="d7126-149">Código de erro</span><span class="sxs-lookup"><span data-stu-id="d7126-149">Error code</span></span>     | <span data-ttu-id="d7126-150">Mensagem de erro</span><span class="sxs-lookup"><span data-stu-id="d7126-150">Error message</span></span>         | <span data-ttu-id="d7126-151">Detalhes</span><span class="sxs-lookup"><span data-stu-id="d7126-151">Details</span></span>             |
|:--------------| :---------------------|:--------------------|
| <span data-ttu-id="d7126-152">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="d7126-152">400 BadRequest</span></span>| <span data-ttu-id="d7126-153">RoleSettingNotFound</span><span class="sxs-lookup"><span data-stu-id="d7126-153">RoleSettingNotFound</span></span>   | <span data-ttu-id="d7126-154">O [governanceRoleSetting](../resources/governancerolesetting.md) não existe no sistema.</span><span class="sxs-lookup"><span data-stu-id="d7126-154">The [governanceRoleSetting](../resources/governancerolesetting.md) does not exist in system.</span></span>
| <span data-ttu-id="d7126-155">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="d7126-155">400 BadRequest</span></span>| <span data-ttu-id="d7126-156">InvalidRoleSetting</span><span class="sxs-lookup"><span data-stu-id="d7126-156">InvalidRoleSetting</span></span>    | <span data-ttu-id="d7126-157">Os valores de [governanceRuleSettings](../resources/governancerulesetting.md) fornecidos no corpo da solicitação não são válidos.</span><span class="sxs-lookup"><span data-stu-id="d7126-157">The [governanceRuleSettings](../resources/governancerulesetting.md) values provided in the request body are not valid.</span></span>

## <a name="example"></a><span data-ttu-id="d7126-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d7126-158">Example</span></span> 
<span data-ttu-id="d7126-159">Este exemplo atualiza a configuração de função para a função 3 personalizada na assinatura Wingtip Toys-prod.</span><span class="sxs-lookup"><span data-stu-id="d7126-159">This example updates the role setting for Custom Role 3 in the subscription Wingtip Toys - Prod.</span></span>
##### <a name="request"></a><span data-ttu-id="d7126-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d7126-160">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="d7126-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="d7126-161">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="d7126-162">C#</span><span class="sxs-lookup"><span data-stu-id="d7126-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-governancerolesetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d7126-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d7126-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-governancerolesetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d7126-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d7126-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-governancerolesetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d7126-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="d7126-165">Response</span></span>
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
