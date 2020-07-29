---
title: Atualizar as ideias
description: Atualizar propriedades do objeto itemInsightsSettings
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: a4072a084b632389296266e54e4c0540da69e8ad
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/29/2020
ms.locfileid: "46509626"
---
# <a name="update-iteminsightssettings"></a><span data-ttu-id="09b12-103">Atualizar itemInsightsSettings</span><span class="sxs-lookup"><span data-stu-id="09b12-103">Update itemInsightsSettings</span></span>

<span data-ttu-id="09b12-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="09b12-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="09b12-105">Atualize as propriedades do recurso [itemInsightsSettings](../resources/iteminsightssettings.md) especificado.</span><span class="sxs-lookup"><span data-stu-id="09b12-105">Update properties of the specified [itemInsightsSettings](../resources/iteminsightssettings.md) resource.</span></span>

<span data-ttu-id="09b12-106">Para saber como personalizar a privacidade do item insights para sua organização, confira [Personalizar a privacidade do insights](/graph/insights-customize-item-insights-privacy?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="09b12-106">To learn how to customize item insights privacy for your organization, see [customize insights privacy](/graph/insights-customize-item-insights-privacy?view=graph-rest-1.0).</span></span> 

## <a name="permissions"></a><span data-ttu-id="09b12-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="09b12-107">Permissions</span></span>

<span data-ttu-id="09b12-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="09b12-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="09b12-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="09b12-110">Permission type</span></span>      | <span data-ttu-id="09b12-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="09b12-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="09b12-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="09b12-112">Delegated (work or school account)</span></span> | <span data-ttu-id="09b12-113">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="09b12-113">User.ReadWrite</span></span> |
|<span data-ttu-id="09b12-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="09b12-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="09b12-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="09b12-115">Not supported.</span></span>    |
|<span data-ttu-id="09b12-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="09b12-116">Application</span></span> | <span data-ttu-id="09b12-117">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="09b12-117">User.ReadWrite</span></span> |

><span data-ttu-id="09b12-118">**Observação:** O uso de permissões delegadas para esta operação exige que o usuário conectado tenha uma função de administrador global.</span><span class="sxs-lookup"><span data-stu-id="09b12-118">**Note:** Using delegated permissions for this operation requires the signed-in user to have a global administrator role.</span></span>

## <a name="http-request"></a><span data-ttu-id="09b12-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="09b12-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

```http
PATCH /organization/{organizationId}/settings/itemInsights
```

## <a name="request-headers"></a><span data-ttu-id="09b12-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="09b12-120">Request headers</span></span>

| <span data-ttu-id="09b12-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="09b12-121">Header</span></span>       | <span data-ttu-id="09b12-122">Valor</span><span class="sxs-lookup"><span data-stu-id="09b12-122">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="09b12-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="09b12-123">Authorization</span></span>  | <span data-ttu-id="09b12-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="09b12-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="09b12-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="09b12-126">Content-Type</span></span>  | <span data-ttu-id="09b12-127">application/json</span><span class="sxs-lookup"><span data-stu-id="09b12-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="09b12-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="09b12-128">Request body</span></span>

<span data-ttu-id="09b12-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="09b12-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="09b12-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="09b12-132">Property</span></span>     | <span data-ttu-id="09b12-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="09b12-133">Type</span></span>   |<span data-ttu-id="09b12-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="09b12-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="09b12-135">isEnabledInOrganization</span><span class="sxs-lookup"><span data-stu-id="09b12-135">isEnabledInOrganization</span></span>|<span data-ttu-id="09b12-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="09b12-136">Boolean</span></span>| <span data-ttu-id="09b12-137">`true`Se o item de organização insights estiver habilitado; `false`se o item de organização insights estiver desabilitado para todos os usuários sem exceções.</span><span class="sxs-lookup"><span data-stu-id="09b12-137">`true` if organization item insights are enabled; `false` if organization item insights are disabled for all users without exceptions.</span></span> <span data-ttu-id="09b12-138">O padrão é `true`.</span><span class="sxs-lookup"><span data-stu-id="09b12-138">Default is `true`.</span></span> <span data-ttu-id="09b12-139">Opcional.</span><span class="sxs-lookup"><span data-stu-id="09b12-139">Optional.</span></span>|
|<span data-ttu-id="09b12-140">disabledForGroup</span><span class="sxs-lookup"><span data-stu-id="09b12-140">disabledForGroup</span></span>|<span data-ttu-id="09b12-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="09b12-141">String</span></span>| <span data-ttu-id="09b12-142">A ID de um grupo do Azure AD, do qual as insights do item dos membros estão desabilitadas.</span><span class="sxs-lookup"><span data-stu-id="09b12-142">The ID of an Azure AD group, of which the members' item insights are disabled.</span></span> <span data-ttu-id="09b12-143">O padrão é `empty`.</span><span class="sxs-lookup"><span data-stu-id="09b12-143">Default is `empty`.</span></span> <span data-ttu-id="09b12-144">Opcional.</span><span class="sxs-lookup"><span data-stu-id="09b12-144">Optional.</span></span>|

## <a name="response"></a><span data-ttu-id="09b12-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="09b12-145">Response</span></span>

<span data-ttu-id="09b12-146">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [itemInsightsSettings](../resources/iteminsightssettings.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="09b12-146">If successful, this method returns a `200 OK` response code and [itemInsightsSettings](../resources/iteminsightssettings.md) object in the response body.</span></span>

><span data-ttu-id="09b12-147">**Observação:** Essa operação verifica a validade dos valores de Propriedade do recurso **itemInsightsSettings** especificado.</span><span class="sxs-lookup"><span data-stu-id="09b12-147">**Note:** This operation verifies the validity of property values of the specified **itemInsightsSettings** resource.</span></span> <span data-ttu-id="09b12-148">Se a propriedade **disabledForGroup** estiver definida, essa operação não verifica a existência do grupo do Azure ad correspondente.</span><span class="sxs-lookup"><span data-stu-id="09b12-148">If the **disabledForGroup** property is set, this operation does not check the existence of the corresponding Azure AD Group.</span></span> <span data-ttu-id="09b12-149">Isso significa que, se você definir **disabledForGroup** como um grupo do Azure AD que não existe ou foi excluído posteriormente, essa operação não será capaz de identificar qualquer associação de grupo e desabilitar insights de item para qualquer usuário específico.</span><span class="sxs-lookup"><span data-stu-id="09b12-149">This means, if you set **disabledForGroup** to an Azure AD group that did not exist or was deleted afterwards, this operation will not be able to identify any group membership and disable item insights for any specific users.</span></span> <span data-ttu-id="09b12-150">Se **isEnabledInOrganization** estiver definido como `true` , a operação habilitará o insights para todos os usuários da organização.</span><span class="sxs-lookup"><span data-stu-id="09b12-150">If **isEnabledInOrganization** is set to `true`, the operation will enable insights for all the users in the organization.</span></span> 

## <a name="example"></a><span data-ttu-id="09b12-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="09b12-151">Example</span></span> 

### <a name="request"></a><span data-ttu-id="09b12-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="09b12-152">Request</span></span>

<span data-ttu-id="09b12-153">Veja a seguir um exemplo de solicitação de como o administrador atualiza a configuração de privacidade "**disabledForGroup**" para proibir a exibição de insights de item de usuários de um grupo específico do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="09b12-153">Here is an example request on how admin updates "**disabledForGroup**" privacy setting in order to prohibit displaying users' item insights of a particular Azure AD group.</span></span>

# <a name="http"></a>[<span data-ttu-id="09b12-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="09b12-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_iteminsightssettings"
}-->

```http
PATCH https://graph.microsoft.com/beta/organization/{organizationId}/settings/itemInsights
Content-type: application/json

{
  "disabledForGroup": "edbfe4fb-ec70-4300-928f-dbb2ae86c981"
}
```
# <a name="javascript"></a>[<span data-ttu-id="09b12-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="09b12-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-iteminsightssettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="09b12-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="09b12-156">Response</span></span>

<span data-ttu-id="09b12-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="09b12-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemInsightsSettings",
  "name": "update_iteminsightssettings"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "isEnabledInOrganization": true,
  "disabledForGroup": "edbfe4fb-ec70-4300-928f-dbb2ae86c981"
}
```
