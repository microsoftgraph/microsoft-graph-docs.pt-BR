---
title: Atualizar governanceRoleSetting
description: Atualize as propriedades de governanceRoleSetting.
ms.openlocfilehash: 2d9417c99e63b1b4c7302c2afdda4c272b2fce82
ms.sourcegitcommit: 82f9d0d10388572a3073b2dde8ca0a7b409135b8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/07/2018
ms.locfileid: "27191113"
---
# <a name="update-governancerolesetting"></a><span data-ttu-id="33b2b-103">Atualizar governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="33b2b-103">Update governanceRoleSetting</span></span>

> <span data-ttu-id="33b2b-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="33b2b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="33b2b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="33b2b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="33b2b-106">Atualize as propriedades de [governanceRoleSetting](../resources/governancerolesetting.md).</span><span class="sxs-lookup"><span data-stu-id="33b2b-106">Update the properties of [governanceRoleSetting](../resources/governancerolesetting.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="33b2b-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="33b2b-107">Permissions</span></span>
<span data-ttu-id="33b2b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="33b2b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="33b2b-110">**Observação:** Essa API também requer que o solicitante tem pelo menos um `Active` atribuição de função de administrador (`owner` ou `user access administrator`) no recurso.</span><span class="sxs-lookup"><span data-stu-id="33b2b-110">**Note:** This API also requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

|<span data-ttu-id="33b2b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="33b2b-111">Permission type</span></span>      | <span data-ttu-id="33b2b-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="33b2b-112">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="33b2b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="33b2b-113">Delegated (work or school account)</span></span> | <span data-ttu-id="33b2b-114">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="33b2b-114">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="33b2b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="33b2b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="33b2b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="33b2b-116">Not supported.</span></span>    |
|<span data-ttu-id="33b2b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="33b2b-117">Application</span></span> | <span data-ttu-id="33b2b-118">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="33b2b-118">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="33b2b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="33b2b-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /privilegedAccess/azureResources/roleSettings/{id}
```
## <a name="request-headers"></a><span data-ttu-id="33b2b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="33b2b-120">Request headers</span></span>
| <span data-ttu-id="33b2b-121">Nome</span><span class="sxs-lookup"><span data-stu-id="33b2b-121">Name</span></span>       | <span data-ttu-id="33b2b-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="33b2b-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="33b2b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="33b2b-123">Authorization</span></span>  | <span data-ttu-id="33b2b-124">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="33b2b-124">Bearer {code}</span></span>|
| <span data-ttu-id="33b2b-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="33b2b-125">Content-type</span></span>  | <span data-ttu-id="33b2b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="33b2b-126">application/json</span></span>|


## <a name="request-body"></a><span data-ttu-id="33b2b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="33b2b-127">Request body</span></span>
<span data-ttu-id="33b2b-128">No corpo da solicitação, forneça os valores para [governanceRuleSettings](../resources/governancerulesetting.md) que precisam ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="33b2b-128">In the request body, supply the values for [governanceRuleSettings](../resources/governancerulesetting.md) that need to be updated.</span></span> 

| <span data-ttu-id="33b2b-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="33b2b-129">Property</span></span>     | <span data-ttu-id="33b2b-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="33b2b-130">Type</span></span>   |<span data-ttu-id="33b2b-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="33b2b-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="33b2b-132">adminEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="33b2b-132">adminEligibleSettings</span></span>|[<span data-ttu-id="33b2b-133">governanceRuleSetting</span><span class="sxs-lookup"><span data-stu-id="33b2b-133">governanceRuleSetting</span></span>](../resources/governancerulesetting.md)|<span data-ttu-id="33b2b-134">As definições de regra que são avaliadas quando um administrador tenta adicionar uma atribuição de função elegíveis.</span><span class="sxs-lookup"><span data-stu-id="33b2b-134">The rule settings that are evaluated when an administrator tries to add an eligible role assignment.</span></span>|
|<span data-ttu-id="33b2b-135">adminMemberSettings</span><span class="sxs-lookup"><span data-stu-id="33b2b-135">adminMemberSettings</span></span>|[<span data-ttu-id="33b2b-136">governanceRuleSetting</span><span class="sxs-lookup"><span data-stu-id="33b2b-136">governanceRuleSetting</span></span>](../resources/governancerulesetting.md)|<span data-ttu-id="33b2b-137">As definições de regra que são avaliadas quando um administrador tenta adicionar uma atribuição de função de membro direto.</span><span class="sxs-lookup"><span data-stu-id="33b2b-137">The rule settings that are evaluated when an administrator tries to add a direct member role assignment.</span></span>|
|<span data-ttu-id="33b2b-138">userEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="33b2b-138">userEligibleSettings</span></span>|[<span data-ttu-id="33b2b-139">governanceRuleSetting</span><span class="sxs-lookup"><span data-stu-id="33b2b-139">governanceRuleSetting</span></span>](../resources/governancerulesetting.md)|<span data-ttu-id="33b2b-140">As definições de regra que são avaliadas quando um usuário tentar adicionar uma atribuição de função elegíveis.</span><span class="sxs-lookup"><span data-stu-id="33b2b-140">The rule settings that are evaluated when a user tries to add an eligible role assignment.</span></span> <span data-ttu-id="33b2b-141">Isso não é suportado para `pimforazurerbac` cenário no momento e podem estar disponíveis nos cenários futuros.</span><span class="sxs-lookup"><span data-stu-id="33b2b-141">This is not supported for `pimforazurerbac` scenario for now, and may be available in the future scenarios.</span></span>|
|<span data-ttu-id="33b2b-142">userMemberSettings</span><span class="sxs-lookup"><span data-stu-id="33b2b-142">userMemberSettings</span></span>|[<span data-ttu-id="33b2b-143">governanceRuleSetting</span><span class="sxs-lookup"><span data-stu-id="33b2b-143">governanceRuleSetting</span></span>](../resources/governancerulesetting.md)|<span data-ttu-id="33b2b-144">As definições de regra que são avaliadas quando um usuário tentar ativar sua atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="33b2b-144">The rule settings that are evaluated when a user tries to activate his role assignment.</span></span>|

## <a name="response"></a><span data-ttu-id="33b2b-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="33b2b-145">Response</span></span>
<span data-ttu-id="33b2b-p104">Se bem-sucedido, este método retorna um código de resposta `204 NoContent`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="33b2b-p104">If successful, this method returns a `204 NoContent` response code. It does not return anything in the response body.</span></span> 

### <a name="error-codes"></a><span data-ttu-id="33b2b-148">Códigos de erro</span><span class="sxs-lookup"><span data-stu-id="33b2b-148">Error codes</span></span>
<span data-ttu-id="33b2b-149">Essa API retorna os códigos de erro HTTP padrão.</span><span class="sxs-lookup"><span data-stu-id="33b2b-149">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="33b2b-150">Além disso, ele retorna os seguintes códigos de erro personalizada.</span><span class="sxs-lookup"><span data-stu-id="33b2b-150">In addition, it returns the following custom error codes.</span></span>

|<span data-ttu-id="33b2b-151">Código de erro</span><span class="sxs-lookup"><span data-stu-id="33b2b-151">Error code</span></span>     | <span data-ttu-id="33b2b-152">Mensagem de erro</span><span class="sxs-lookup"><span data-stu-id="33b2b-152">Error message</span></span>         | <span data-ttu-id="33b2b-153">Detalhes</span><span class="sxs-lookup"><span data-stu-id="33b2b-153">Details</span></span>             |
|:--------------| :---------------------|:--------------------|
| <span data-ttu-id="33b2b-154">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="33b2b-154">400 BadRequest</span></span>| <span data-ttu-id="33b2b-155">RoleSettingNotFound</span><span class="sxs-lookup"><span data-stu-id="33b2b-155">RoleSettingNotFound</span></span>   | <span data-ttu-id="33b2b-156">O [governanceRoleSetting](../resources/governancerolesetting.md) não existe no sistema.</span><span class="sxs-lookup"><span data-stu-id="33b2b-156">The [governanceRoleSetting](../resources/governancerolesetting.md) does not exist in system.</span></span>
| <span data-ttu-id="33b2b-157">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="33b2b-157">400 BadRequest</span></span>| <span data-ttu-id="33b2b-158">InvalidRoleSetting</span><span class="sxs-lookup"><span data-stu-id="33b2b-158">InvalidRoleSetting</span></span>    | <span data-ttu-id="33b2b-159">Os valores de [governanceRuleSettings](../resources/governancerulesetting.md) fornecidos no corpo da solicitação não são válidos.</span><span class="sxs-lookup"><span data-stu-id="33b2b-159">The [governanceRuleSettings](../resources/governancerulesetting.md) values provided in the request body are not valid.</span></span>

## <a name="example"></a><span data-ttu-id="33b2b-160">Exemplo</span><span class="sxs-lookup"><span data-stu-id="33b2b-160">Example</span></span> 
<span data-ttu-id="33b2b-161">Este exemplo atualiza a definição de função para 3 de função personalizada na assinatura Wingtip Toys - produção.</span><span class="sxs-lookup"><span data-stu-id="33b2b-161">This example updates the role setting for Custom Role 3 in the subscription Wingtip Toys - Prod.</span></span>
##### <a name="request"></a><span data-ttu-id="33b2b-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="33b2b-162">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="33b2b-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="33b2b-163">Response</span></span>
<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update governanceRoleSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
