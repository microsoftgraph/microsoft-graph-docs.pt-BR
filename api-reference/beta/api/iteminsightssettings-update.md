---
title: Atualizar itemInsights
description: Atualizar propriedades do objeto itemInsightsSettings
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: 0eb17d9e0a4f3285858800f32e6954bbd344dc27
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053031"
---
# <a name="update-iteminsightssettings"></a><span data-ttu-id="cf1b7-103">Atualizar itemInsightsSettings</span><span class="sxs-lookup"><span data-stu-id="cf1b7-103">Update itemInsightsSettings</span></span>

<span data-ttu-id="cf1b7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cf1b7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cf1b7-105">Atualizar propriedades do recurso [itemInsightsSettings](../resources/iteminsightssettings.md) especificado.</span><span class="sxs-lookup"><span data-stu-id="cf1b7-105">Update properties of the specified [itemInsightsSettings](../resources/iteminsightssettings.md) resource.</span></span>

<span data-ttu-id="cf1b7-106">Para saber como personalizar a privacidade de insights de item para sua organização, consulte [personalizar a privacidade de insights.](/graph/insights-customize-item-insights-privacy?view=graph-rest-1.0)</span><span class="sxs-lookup"><span data-stu-id="cf1b7-106">To learn how to customize item insights privacy for your organization, see [customize insights privacy](/graph/insights-customize-item-insights-privacy?view=graph-rest-1.0).</span></span> 

## <a name="permissions"></a><span data-ttu-id="cf1b7-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="cf1b7-107">Permissions</span></span>

<span data-ttu-id="cf1b7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cf1b7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf1b7-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cf1b7-110">Permission type</span></span>      | <span data-ttu-id="cf1b7-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cf1b7-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cf1b7-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cf1b7-112">Delegated (work or school account)</span></span> | <span data-ttu-id="cf1b7-113">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf1b7-113">User.ReadWrite.All</span></span> |
|<span data-ttu-id="cf1b7-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cf1b7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cf1b7-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cf1b7-115">Not supported.</span></span>    |
|<span data-ttu-id="cf1b7-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cf1b7-116">Application</span></span> | <span data-ttu-id="cf1b7-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cf1b7-117">Not supported.</span></span> |

><span data-ttu-id="cf1b7-118">**Observação:** O uso de permissões delegadas para essa operação exige que o usuário inscreveu tenha uma função de administrador global.</span><span class="sxs-lookup"><span data-stu-id="cf1b7-118">**Note:** Using delegated permissions for this operation requires the signed-in user to have a global administrator role.</span></span>

## <a name="http-request"></a><span data-ttu-id="cf1b7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cf1b7-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

```http
PATCH /organization/{organizationId}/settings/itemInsights
```

## <a name="request-headers"></a><span data-ttu-id="cf1b7-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cf1b7-120">Request headers</span></span>

| <span data-ttu-id="cf1b7-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cf1b7-121">Header</span></span>       | <span data-ttu-id="cf1b7-122">Valor</span><span class="sxs-lookup"><span data-stu-id="cf1b7-122">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="cf1b7-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="cf1b7-123">Authorization</span></span>  | <span data-ttu-id="cf1b7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cf1b7-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="cf1b7-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cf1b7-126">Content-Type</span></span>  | <span data-ttu-id="cf1b7-127">application/json</span><span class="sxs-lookup"><span data-stu-id="cf1b7-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cf1b7-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cf1b7-128">Request body</span></span>

<span data-ttu-id="cf1b7-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="cf1b7-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="cf1b7-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cf1b7-132">Property</span></span>     | <span data-ttu-id="cf1b7-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="cf1b7-133">Type</span></span>   |<span data-ttu-id="cf1b7-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="cf1b7-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cf1b7-135">isEnabledInOrganization</span><span class="sxs-lookup"><span data-stu-id="cf1b7-135">isEnabledInOrganization</span></span>|<span data-ttu-id="cf1b7-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="cf1b7-136">Boolean</span></span>| <span data-ttu-id="cf1b7-137">`true` se as percepções do item da organização estão habilitadas; `false` se as percepções do item da organização estão desabilitadas para todos os usuários sem exceções.</span><span class="sxs-lookup"><span data-stu-id="cf1b7-137">`true` if organization item insights are enabled; `false` if organization item insights are disabled for all users without exceptions.</span></span> <span data-ttu-id="cf1b7-138">O padrão é `true`.</span><span class="sxs-lookup"><span data-stu-id="cf1b7-138">Default is `true`.</span></span> <span data-ttu-id="cf1b7-139">Opcional.</span><span class="sxs-lookup"><span data-stu-id="cf1b7-139">Optional.</span></span>|
|<span data-ttu-id="cf1b7-140">disabledForGroup</span><span class="sxs-lookup"><span data-stu-id="cf1b7-140">disabledForGroup</span></span>|<span data-ttu-id="cf1b7-141">String</span><span class="sxs-lookup"><span data-stu-id="cf1b7-141">String</span></span>| <span data-ttu-id="cf1b7-142">A ID de um grupo do Azure AD, do qual as informações do item dos membros estão desabilitadas.</span><span class="sxs-lookup"><span data-stu-id="cf1b7-142">The ID of an Azure AD group, of which the members' item insights are disabled.</span></span> <span data-ttu-id="cf1b7-143">O padrão é `empty`.</span><span class="sxs-lookup"><span data-stu-id="cf1b7-143">Default is `empty`.</span></span> <span data-ttu-id="cf1b7-144">Opcional.</span><span class="sxs-lookup"><span data-stu-id="cf1b7-144">Optional.</span></span>|

## <a name="response"></a><span data-ttu-id="cf1b7-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="cf1b7-145">Response</span></span>

<span data-ttu-id="cf1b7-146">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [itemInsightsSettings](../resources/iteminsightssettings.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cf1b7-146">If successful, this method returns a `200 OK` response code and [itemInsightsSettings](../resources/iteminsightssettings.md) object in the response body.</span></span>

><span data-ttu-id="cf1b7-147">**Observação:** Esta operação verifica a validade dos valores de propriedade do **recurso itemInsightsSettings** especificado.</span><span class="sxs-lookup"><span data-stu-id="cf1b7-147">**Note:** This operation verifies the validity of property values of the specified **itemInsightsSettings** resource.</span></span> <span data-ttu-id="cf1b7-148">Se a **propriedade disabledForGroup** estiver definida, essa operação não verificará a existência do Grupo do Azure AD correspondente.</span><span class="sxs-lookup"><span data-stu-id="cf1b7-148">If the **disabledForGroup** property is set, this operation does not check the existence of the corresponding Azure AD Group.</span></span> <span data-ttu-id="cf1b7-149">Isso significa que, se você definir **disabledForGroup** para um grupo do Azure AD que não existia ou foi excluído posteriormente, essa operação não poderá identificar nenhuma associação de grupo e desabilitar informações de item para usuários específicos.</span><span class="sxs-lookup"><span data-stu-id="cf1b7-149">This means, if you set **disabledForGroup** to an Azure AD group that did not exist or was deleted afterwards, this operation will not be able to identify any group membership and disable item insights for any specific users.</span></span> <span data-ttu-id="cf1b7-150">Se **isEnabledInOrganization** estiver definido como , a operação permitirá insights `true` para todos os usuários na organização.</span><span class="sxs-lookup"><span data-stu-id="cf1b7-150">If **isEnabledInOrganization** is set to `true`, the operation will enable insights for all the users in the organization.</span></span> 

## <a name="example"></a><span data-ttu-id="cf1b7-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cf1b7-151">Example</span></span> 

### <a name="request"></a><span data-ttu-id="cf1b7-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cf1b7-152">Request</span></span>

<span data-ttu-id="cf1b7-153">Aqui está um exemplo de solicitação sobre como o administrador atualiza a configuração de privacidade "**disabledForGroup**" para proibir a exibição de informações de item dos usuários de um grupo específico do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="cf1b7-153">Here is an example request on how admin updates "**disabledForGroup**" privacy setting in order to prohibit displaying users' item insights of a particular Azure AD group.</span></span>

# <a name="http"></a>[<span data-ttu-id="cf1b7-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="cf1b7-154">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="cf1b7-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cf1b7-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-iteminsightssettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="cf1b7-156">C#</span><span class="sxs-lookup"><span data-stu-id="cf1b7-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-iteminsightssettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cf1b7-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cf1b7-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-iteminsightssettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cf1b7-158">Java</span><span class="sxs-lookup"><span data-stu-id="cf1b7-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-iteminsightssettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="cf1b7-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="cf1b7-159">Response</span></span>

<span data-ttu-id="cf1b7-160">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cf1b7-160">Here is an example of the response.</span></span> <span data-ttu-id="cf1b7-161">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="cf1b7-161">Note: The response object shown here might be shortened for readability.</span></span>
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


