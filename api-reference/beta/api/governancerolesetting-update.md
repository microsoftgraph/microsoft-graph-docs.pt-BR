---
title: Atualizar governanceRoleSetting
description: Atualize as propriedades de governanceRoleSetting.
localization_priority: Normal
ms.openlocfilehash: e5fc297690816227e1031af363ea7d4d38199e25
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509326"
---
# <a name="update-governancerolesetting"></a><span data-ttu-id="b84c7-103">Atualizar governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="b84c7-103">Update governanceRoleSetting</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b84c7-104">Atualize as propriedades de [governanceRoleSetting](../resources/governancerolesetting.md).</span><span class="sxs-lookup"><span data-stu-id="b84c7-104">Update the properties of [governanceRoleSetting](../resources/governancerolesetting.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b84c7-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="b84c7-105">Permissions</span></span>
<span data-ttu-id="b84c7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b84c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="b84c7-108">**Observação:** Essa API também requer que o solicitante tem pelo menos um `Active` atribuição de função de administrador (`owner` ou `user access administrator`) no recurso.</span><span class="sxs-lookup"><span data-stu-id="b84c7-108">**Note:** This API also requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

|<span data-ttu-id="b84c7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b84c7-109">Permission type</span></span>      | <span data-ttu-id="b84c7-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="b84c7-110">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b84c7-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b84c7-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b84c7-112">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="b84c7-112">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="b84c7-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b84c7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b84c7-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b84c7-114">Not supported.</span></span>    |
|<span data-ttu-id="b84c7-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b84c7-115">Application</span></span> | <span data-ttu-id="b84c7-116">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="b84c7-116">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="b84c7-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b84c7-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /privilegedAccess/azureResources/roleSettings/{id}
```
## <a name="request-headers"></a><span data-ttu-id="b84c7-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b84c7-118">Request headers</span></span>
| <span data-ttu-id="b84c7-119">Nome</span><span class="sxs-lookup"><span data-stu-id="b84c7-119">Name</span></span>       | <span data-ttu-id="b84c7-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="b84c7-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="b84c7-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="b84c7-121">Authorization</span></span>  | <span data-ttu-id="b84c7-122">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="b84c7-122">Bearer {code}</span></span>|
| <span data-ttu-id="b84c7-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="b84c7-123">Content-type</span></span>  | <span data-ttu-id="b84c7-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b84c7-124">application/json</span></span>|


## <a name="request-body"></a><span data-ttu-id="b84c7-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b84c7-125">Request body</span></span>
<span data-ttu-id="b84c7-126">No corpo da solicitação, forneça os valores para [governanceRuleSettings](../resources/governancerulesetting.md) que precisam ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="b84c7-126">In the request body, supply the values for [governanceRuleSettings](../resources/governancerulesetting.md) that need to be updated.</span></span> 

| <span data-ttu-id="b84c7-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b84c7-127">Property</span></span>     | <span data-ttu-id="b84c7-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="b84c7-128">Type</span></span>   |<span data-ttu-id="b84c7-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="b84c7-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b84c7-130">adminEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="b84c7-130">adminEligibleSettings</span></span>|[<span data-ttu-id="b84c7-131">governanceRuleSetting</span><span class="sxs-lookup"><span data-stu-id="b84c7-131">governanceRuleSetting</span></span>](../resources/governancerulesetting.md)|<span data-ttu-id="b84c7-132">As definições de regra que são avaliadas quando um administrador tenta adicionar uma atribuição de função elegíveis.</span><span class="sxs-lookup"><span data-stu-id="b84c7-132">The rule settings that are evaluated when an administrator tries to add an eligible role assignment.</span></span>|
|<span data-ttu-id="b84c7-133">adminMemberSettings</span><span class="sxs-lookup"><span data-stu-id="b84c7-133">adminMemberSettings</span></span>|[<span data-ttu-id="b84c7-134">governanceRuleSetting</span><span class="sxs-lookup"><span data-stu-id="b84c7-134">governanceRuleSetting</span></span>](../resources/governancerulesetting.md)|<span data-ttu-id="b84c7-135">As definições de regra que são avaliadas quando um administrador tenta adicionar uma atribuição de função de membro direto.</span><span class="sxs-lookup"><span data-stu-id="b84c7-135">The rule settings that are evaluated when an administrator tries to add a direct member role assignment.</span></span>|
|<span data-ttu-id="b84c7-136">userEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="b84c7-136">userEligibleSettings</span></span>|[<span data-ttu-id="b84c7-137">governanceRuleSetting</span><span class="sxs-lookup"><span data-stu-id="b84c7-137">governanceRuleSetting</span></span>](../resources/governancerulesetting.md)|<span data-ttu-id="b84c7-138">As definições de regra que são avaliadas quando um usuário tentar adicionar uma atribuição de função elegíveis.</span><span class="sxs-lookup"><span data-stu-id="b84c7-138">The rule settings that are evaluated when a user tries to add an eligible role assignment.</span></span> <span data-ttu-id="b84c7-139">Isso não é suportado para `pimforazurerbac` cenário no momento e podem estar disponíveis nos cenários futuros.</span><span class="sxs-lookup"><span data-stu-id="b84c7-139">This is not supported for `pimforazurerbac` scenario for now, and may be available in the future scenarios.</span></span>|
|<span data-ttu-id="b84c7-140">userMemberSettings</span><span class="sxs-lookup"><span data-stu-id="b84c7-140">userMemberSettings</span></span>|[<span data-ttu-id="b84c7-141">governanceRuleSetting</span><span class="sxs-lookup"><span data-stu-id="b84c7-141">governanceRuleSetting</span></span>](../resources/governancerulesetting.md)|<span data-ttu-id="b84c7-142">As definições de regra que são avaliadas quando um usuário tentar ativar sua atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="b84c7-142">The rule settings that are evaluated when a user tries to activate his role assignment.</span></span>|

## <a name="response"></a><span data-ttu-id="b84c7-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="b84c7-143">Response</span></span>
<span data-ttu-id="b84c7-p103">Se bem-sucedido, este método retorna um código de resposta `204 NoContent`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b84c7-p103">If successful, this method returns a `204 NoContent` response code. It does not return anything in the response body.</span></span> 

### <a name="error-codes"></a><span data-ttu-id="b84c7-146">Códigos de erro</span><span class="sxs-lookup"><span data-stu-id="b84c7-146">Error codes</span></span>
<span data-ttu-id="b84c7-147">Essa API retorna os códigos de erro HTTP padrão.</span><span class="sxs-lookup"><span data-stu-id="b84c7-147">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="b84c7-148">Além disso, ele retorna os seguintes códigos de erro personalizada.</span><span class="sxs-lookup"><span data-stu-id="b84c7-148">In addition, it returns the following custom error codes.</span></span>

|<span data-ttu-id="b84c7-149">Código de erro</span><span class="sxs-lookup"><span data-stu-id="b84c7-149">Error code</span></span>     | <span data-ttu-id="b84c7-150">Mensagem de erro</span><span class="sxs-lookup"><span data-stu-id="b84c7-150">Error message</span></span>         | <span data-ttu-id="b84c7-151">Detalhes</span><span class="sxs-lookup"><span data-stu-id="b84c7-151">Details</span></span>             |
|:--------------| :---------------------|:--------------------|
| <span data-ttu-id="b84c7-152">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="b84c7-152">400 BadRequest</span></span>| <span data-ttu-id="b84c7-153">RoleSettingNotFound</span><span class="sxs-lookup"><span data-stu-id="b84c7-153">RoleSettingNotFound</span></span>   | <span data-ttu-id="b84c7-154">O [governanceRoleSetting](../resources/governancerolesetting.md) não existe no sistema.</span><span class="sxs-lookup"><span data-stu-id="b84c7-154">The [governanceRoleSetting](../resources/governancerolesetting.md) does not exist in system.</span></span>
| <span data-ttu-id="b84c7-155">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="b84c7-155">400 BadRequest</span></span>| <span data-ttu-id="b84c7-156">InvalidRoleSetting</span><span class="sxs-lookup"><span data-stu-id="b84c7-156">InvalidRoleSetting</span></span>    | <span data-ttu-id="b84c7-157">Os valores de [governanceRuleSettings](../resources/governancerulesetting.md) fornecidos no corpo da solicitação não são válidos.</span><span class="sxs-lookup"><span data-stu-id="b84c7-157">The [governanceRuleSettings](../resources/governancerulesetting.md) values provided in the request body are not valid.</span></span>

## <a name="example"></a><span data-ttu-id="b84c7-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b84c7-158">Example</span></span> 
<span data-ttu-id="b84c7-159">Este exemplo atualiza a definição de função para 3 de função personalizada na assinatura Wingtip Toys - produção.</span><span class="sxs-lookup"><span data-stu-id="b84c7-159">This example updates the role setting for Custom Role 3 in the subscription Wingtip Toys - Prod.</span></span>
##### <a name="request"></a><span data-ttu-id="b84c7-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b84c7-160">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "update_governancerolesetting"
}-->
```http
PATCH https://graph.microsoft.com/beta/privilegedAccess/pimforazurerbac/roleSettings/5fb5aef8-1081-4b8e-bb16-9d5d0385bab5
Content-type: application/json
Content-length: 350

{
  "adminEligibleSettings":[{"ruleIdentifier":"ExpirationRule","setting":"{\"permanentAssignment\":false,\"maximumGrantPeriodInMinutes\":129600}"}]
}
```
##### <a name="response"></a><span data-ttu-id="b84c7-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="b84c7-161">Response</span></span>
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
    "Error: /api-reference/beta/api/governancerolesetting-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
