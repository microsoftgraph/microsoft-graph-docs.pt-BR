---
title: Atualizar governanceRoleSetting
description: Atualize as propriedades de governanceRoleSetting.
ms.openlocfilehash: ca5752d51e5d59578594a12c80ae1cac316b48bc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033383"
---
# <a name="update-governancerolesetting"></a><span data-ttu-id="e8383-103">Atualizar governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="e8383-103">Update governanceRoleSetting</span></span>

> <span data-ttu-id="e8383-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e8383-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e8383-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e8383-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e8383-106">Atualize as propriedades de [governanceRoleSetting](../resources/governancerolesetting.md).</span><span class="sxs-lookup"><span data-stu-id="e8383-106">Update the properties of [governanceRoleSetting](../resources/governancerolesetting.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e8383-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="e8383-107">Permissions</span></span>
<span data-ttu-id="e8383-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8383-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8383-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e8383-110">Permission type</span></span>      | <span data-ttu-id="e8383-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="e8383-111">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e8383-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e8383-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e8383-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="e8383-113">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="e8383-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e8383-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e8383-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e8383-115">Not supported.</span></span>    |
|<span data-ttu-id="e8383-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e8383-116">Application</span></span> | <span data-ttu-id="e8383-117">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="e8383-117">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

<span data-ttu-id="e8383-118">Além do escopo de permissão, essa API requer o solicitante ter pelo menos um `Active` atribuição de função de administrador (`owner` ou `user access administrator`) no recurso.</span><span class="sxs-lookup"><span data-stu-id="e8383-118">Besides the permission scope, this API requires the requestor to have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>
## <a name="http-request"></a><span data-ttu-id="e8383-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e8383-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /privilegedAccess/azureResources/roleSettings/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="e8383-120">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="e8383-120">Optional request headers</span></span>
| <span data-ttu-id="e8383-121">Nome</span><span class="sxs-lookup"><span data-stu-id="e8383-121">Name</span></span>       | <span data-ttu-id="e8383-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="e8383-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="e8383-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e8383-123">Authorization</span></span>  | <span data-ttu-id="e8383-124">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="e8383-124">Bearer {code}</span></span>|
| <span data-ttu-id="e8383-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="e8383-125">Content-type</span></span>  | <span data-ttu-id="e8383-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e8383-126">application/json</span></span>|


## <a name="request-body"></a><span data-ttu-id="e8383-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e8383-127">Request body</span></span>
<span data-ttu-id="e8383-128">No corpo da solicitação, forneça os valores para [governanceRuleSettings](../resources/governancerulesetting.md) que precisa ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="e8383-128">In the request body, supply the values for [governanceRuleSettings](../resources/governancerulesetting.md) that needs to be updated.</span></span> 

| <span data-ttu-id="e8383-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e8383-129">Property</span></span>     | <span data-ttu-id="e8383-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="e8383-130">Type</span></span>   |<span data-ttu-id="e8383-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="e8383-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e8383-132">adminEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="e8383-132">adminEligibleSettings</span></span>|[<span data-ttu-id="e8383-133">governanceRuleSetting</span><span class="sxs-lookup"><span data-stu-id="e8383-133">governanceRuleSetting</span></span>](../resources/governancerulesetting.md)|<span data-ttu-id="e8383-134">As definições de regra que são avaliadas quando um administrador tenta adicionar uma atribuição de função elegíveis.</span><span class="sxs-lookup"><span data-stu-id="e8383-134">The rule settings that are evaluated when an administrator tries to add an eligible role assignment.</span></span>|
|<span data-ttu-id="e8383-135">adminMemberSettings</span><span class="sxs-lookup"><span data-stu-id="e8383-135">adminMemberSettings</span></span>|[<span data-ttu-id="e8383-136">governanceRuleSetting</span><span class="sxs-lookup"><span data-stu-id="e8383-136">governanceRuleSetting</span></span>](../resources/governancerulesetting.md)|<span data-ttu-id="e8383-137">As definições de regra que são avaliadas quando um administrador tenta adicionar uma atribuição de função de membro direto.</span><span class="sxs-lookup"><span data-stu-id="e8383-137">The rule settings that are evaluated when an administrator tries to add a direct member role assignment.</span></span>|
|<span data-ttu-id="e8383-138">userEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="e8383-138">userEligibleSettings</span></span>|[<span data-ttu-id="e8383-139">governanceRuleSetting</span><span class="sxs-lookup"><span data-stu-id="e8383-139">governanceRuleSetting</span></span>](../resources/governancerulesetting.md)|<span data-ttu-id="e8383-140">As definições de regra que são avaliadas quando um usuário tentar adicionar uma atribuição de função elegíveis.</span><span class="sxs-lookup"><span data-stu-id="e8383-140">The rule settings that are evaluated when a user tries to add an eligible role assignment.</span></span> <span data-ttu-id="e8383-141">Isso não é suportado para `pimforazurerbac` cenário no momento e podem estar disponíveis nos cenários futuros.</span><span class="sxs-lookup"><span data-stu-id="e8383-141">This is not supported for `pimforazurerbac` scenario for now, and may be available in the future scenarios.</span></span>|
|<span data-ttu-id="e8383-142">userMemberSettings</span><span class="sxs-lookup"><span data-stu-id="e8383-142">userMemberSettings</span></span>|[<span data-ttu-id="e8383-143">governanceRuleSetting</span><span class="sxs-lookup"><span data-stu-id="e8383-143">governanceRuleSetting</span></span>](../resources/governancerulesetting.md)|<span data-ttu-id="e8383-144">As definições de regra que são avaliadas quando um usuário tentar ativar sua atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="e8383-144">The rule settings that are evaluated when a user tries to activate his role assignment.</span></span>|

## <a name="response"></a><span data-ttu-id="e8383-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8383-145">Response</span></span>
<span data-ttu-id="e8383-p104">Se bem-sucedido, este método retorna um código de resposta `204 NoContent`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e8383-p104">If successful, this method returns `204 NoContent` response code. It does not return anything in the response body.</span></span> 

## <a name="error-codes"></a><span data-ttu-id="e8383-148">Códigos de erro</span><span class="sxs-lookup"><span data-stu-id="e8383-148">Error codes</span></span>
<span data-ttu-id="e8383-149">Essa API segue o padrão dos códigos HTTP.</span><span class="sxs-lookup"><span data-stu-id="e8383-149">This API follows the standard of HTTP codes.</span></span> <span data-ttu-id="e8383-150">Além disso, os códigos de erro personalizadas são mostrados abaixo.</span><span class="sxs-lookup"><span data-stu-id="e8383-150">Besides, the custom error codes are shown below.</span></span>
|<span data-ttu-id="e8383-151">Código de erro</span><span class="sxs-lookup"><span data-stu-id="e8383-151">Error code</span></span>     | <span data-ttu-id="e8383-152">Mensagem de erro</span><span class="sxs-lookup"><span data-stu-id="e8383-152">Error message</span></span>         | <span data-ttu-id="e8383-153">Detalhes</span><span class="sxs-lookup"><span data-stu-id="e8383-153">Details</span></span>             |
|:--------------| :---------------------|:--------------------|
| <span data-ttu-id="e8383-154">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="e8383-154">400 BadRequest</span></span>| <span data-ttu-id="e8383-155">RoleSettingNotFound</span><span class="sxs-lookup"><span data-stu-id="e8383-155">RoleSettingNotFound</span></span>   | <span data-ttu-id="e8383-156">O [governanceRoleSetting](../resources/governancerolesetting.md) não existe no sistema.</span><span class="sxs-lookup"><span data-stu-id="e8383-156">The [governanceRoleSetting](../resources/governancerolesetting.md) does not exist in system.</span></span>
| <span data-ttu-id="e8383-157">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="e8383-157">400 BadRequest</span></span>| <span data-ttu-id="e8383-158">InvalidRoleSetting</span><span class="sxs-lookup"><span data-stu-id="e8383-158">InvalidRoleSetting</span></span>    | <span data-ttu-id="e8383-159">Os valores de [governanceRuleSettings](../resources/governancerulesetting.md) fornecidos no corpo da solicitação não são válidos.</span><span class="sxs-lookup"><span data-stu-id="e8383-159">The [governanceRuleSettings](../resources/governancerulesetting.md) values provided in the request body are not valid.</span></span>

## <a name="example"></a><span data-ttu-id="e8383-160">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e8383-160">Example</span></span> 
<span data-ttu-id="e8383-161">Este exemplo atualiza a definição de função para 3 de função personalizada na assinatura Wingtip Toys - produção.</span><span class="sxs-lookup"><span data-stu-id="e8383-161">This example updates the role setting for Custom Role 3 in the subscription Wingtip Toys - Prod.</span></span>
##### <a name="request"></a><span data-ttu-id="e8383-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e8383-162">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="e8383-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8383-163">Response</span></span>
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
