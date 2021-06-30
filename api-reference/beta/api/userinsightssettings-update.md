---
title: Atualizar userInsightsSettings
description: Atualize as propriedades de um objeto userInsightsSettings.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: a422a106d1371e8e39fdfa314658b8e77d0f5a9a
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53210652"
---
# <a name="update-userinsightssettings"></a><span data-ttu-id="03019-103">Atualizar userInsightsSettings</span><span class="sxs-lookup"><span data-stu-id="03019-103">Update userInsightsSettings</span></span>

<span data-ttu-id="03019-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="03019-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="03019-105">Atualize as configurações de privacidade [para itemInsights](../resources/iteminsights.md) e informações de horários [de reunião](https://support.microsoft.com/en-us/office/update-your-meeting-hours-using-the-profile-card-0613d113-d7c1-4faa-bb11-c8ba30a78ef1) de um usuário.</span><span class="sxs-lookup"><span data-stu-id="03019-105">Update the privacy settings for [itemInsights](../resources/iteminsights.md) and [meeting hours insights](https://support.microsoft.com/en-us/office/update-your-meeting-hours-using-the-profile-card-0613d113-d7c1-4faa-bb11-c8ba30a78ef1) of a user.</span></span>

## <a name="permissions"></a><span data-ttu-id="03019-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="03019-106">Permissions</span></span>

<span data-ttu-id="03019-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="03019-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03019-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="03019-109">Permission type</span></span>      | <span data-ttu-id="03019-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="03019-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="03019-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="03019-111">Delegated (work or school account)</span></span> | <span data-ttu-id="03019-112">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="03019-112">User.ReadWrite</span></span> |
|<span data-ttu-id="03019-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="03019-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="03019-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="03019-114">Not supported.</span></span>    |
|<span data-ttu-id="03019-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="03019-115">Application</span></span> | <span data-ttu-id="03019-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="03019-116">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="03019-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="03019-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/settings/itemInsights
PATCH /users/{userId}/settings/itemInsights
```

><span data-ttu-id="03019-118">**Observação:** As solicitações com um ou são acessíveis apenas pelo usuário ou por um usuário com as permissões `userId` `userPrincipalName` User.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="03019-118">**Note:** Requests with a `userId` or `userPrincipalName` are only accessible by the user or by a user with the User.ReadWrite.All permissions.</span></span> <span data-ttu-id="03019-119">Para saber mais, confira [permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="03019-119">To learn more, see [Permissions](/graph/permissions-reference).</span></span>

## <a name="request-headers"></a><span data-ttu-id="03019-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="03019-120">Request headers</span></span>

| <span data-ttu-id="03019-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="03019-121">Header</span></span>       | <span data-ttu-id="03019-122">Valor</span><span class="sxs-lookup"><span data-stu-id="03019-122">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="03019-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="03019-123">Authorization</span></span>  | <span data-ttu-id="03019-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="03019-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="03019-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="03019-126">Content-Type</span></span>  | <span data-ttu-id="03019-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="03019-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="03019-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="03019-129">Request body</span></span>

<span data-ttu-id="03019-p105">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="03019-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="03019-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="03019-133">Property</span></span>     | <span data-ttu-id="03019-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="03019-134">Type</span></span>   |<span data-ttu-id="03019-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="03019-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="03019-136">isEnabled</span><span class="sxs-lookup"><span data-stu-id="03019-136">isEnabled</span></span>|<span data-ttu-id="03019-137">Booliano</span><span class="sxs-lookup"><span data-stu-id="03019-137">Boolean</span></span>| <span data-ttu-id="03019-138">`true` se os insights **de item do usuárioInsights** e de horas de reunião estão habilitados; `false` se o item do **usuárioInights** e as percepções do horário de reunião estão desabilitados.</span><span class="sxs-lookup"><span data-stu-id="03019-138">`true` if user's **itemInsights** and meeting hours insights are enabled; `false` if user's **itemInsights** and meeting hours insights are disabled.</span></span> <span data-ttu-id="03019-139">O padrão é `true`.</span><span class="sxs-lookup"><span data-stu-id="03019-139">Default is `true`.</span></span> <span data-ttu-id="03019-140">Opcional.</span><span class="sxs-lookup"><span data-stu-id="03019-140">Optional.</span></span>|

## <a name="response"></a><span data-ttu-id="03019-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="03019-141">Response</span></span>

<span data-ttu-id="03019-142">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto userInsightsSettings](../resources/userinsightssettings.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="03019-142">If successful, this method returns a `200 OK` response code and [userInsightsSettings](../resources/userinsightssettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="03019-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="03019-143">Example</span></span> 

### <a name="request"></a><span data-ttu-id="03019-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="03019-144">Request</span></span>

<span data-ttu-id="03019-145">Veja a seguir uma solicitação de exemplo sobre como o usuário atualiza a configuração de privacidade "**isEnabled**" para desabilitar suas percepções de item e informações do horário de reunião.</span><span class="sxs-lookup"><span data-stu-id="03019-145">The following is an example request on how user updates "**isEnabled**" privacy setting in order to disable his item insights and meeting hours insights.</span></span>


# <a name="http"></a>[<span data-ttu-id="03019-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="03019-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_userInsightsSettings"
}-->

```http
PATCH https://graph.microsoft.com/beta/users/{userId}/settings/itemInsights
Content-type: application/json

{
  "isEnabled": "false"
}
```
# <a name="c"></a>[<span data-ttu-id="03019-147">C#</span><span class="sxs-lookup"><span data-stu-id="03019-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-userinsightssettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="03019-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="03019-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-userinsightssettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="03019-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="03019-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-userinsightssettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="03019-150">Java</span><span class="sxs-lookup"><span data-stu-id="03019-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-userinsightssettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="03019-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="03019-151">Response</span></span>

<span data-ttu-id="03019-152">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="03019-152">The following is an example of the response.</span></span> 

><span data-ttu-id="03019-153">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="03019-153">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userInsightsSettings",
  "name": "update_userInsightsSettings"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "isEnabled": false,
}
```
