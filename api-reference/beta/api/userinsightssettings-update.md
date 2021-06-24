---
title: Atualizar userInsightsSettings
description: Atualize as propriedades de um objeto userInsightsSettings.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: 5f161d5b75e862f358d07fee2347bb3f4d18bbad
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2021
ms.locfileid: "53107791"
---
# <a name="update-userinsightssettings"></a><span data-ttu-id="bf323-103">Atualizar userInsightsSettings</span><span class="sxs-lookup"><span data-stu-id="bf323-103">Update userInsightsSettings</span></span>

<span data-ttu-id="bf323-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bf323-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bf323-105">Atualize as configurações de privacidade [para itemInsights](../resources/iteminsights.md) e informações de horários [de reunião](https://support.microsoft.com/en-us/office/update-your-meeting-hours-using-the-profile-card-0613d113-d7c1-4faa-bb11-c8ba30a78ef1) de um usuário.</span><span class="sxs-lookup"><span data-stu-id="bf323-105">Update the privacy settings for [itemInsights](../resources/iteminsights.md) and [meeting hours insights](https://support.microsoft.com/en-us/office/update-your-meeting-hours-using-the-profile-card-0613d113-d7c1-4faa-bb11-c8ba30a78ef1) of a user.</span></span>

## <a name="permissions"></a><span data-ttu-id="bf323-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="bf323-106">Permissions</span></span>

<span data-ttu-id="bf323-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bf323-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bf323-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bf323-109">Permission type</span></span>      | <span data-ttu-id="bf323-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bf323-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bf323-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bf323-111">Delegated (work or school account)</span></span> | <span data-ttu-id="bf323-112">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bf323-112">User.ReadWrite</span></span> |
|<span data-ttu-id="bf323-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bf323-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bf323-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bf323-114">Not supported.</span></span>    |
|<span data-ttu-id="bf323-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bf323-115">Application</span></span> | <span data-ttu-id="bf323-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bf323-116">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="bf323-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bf323-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/settings/itemInsights
PATCH /users/{userId}/settings/itemInsights
```

><span data-ttu-id="bf323-118">**Observação:** As solicitações com um ou são acessíveis apenas pelo usuário ou por um usuário com as permissões `userId` `userPrincipalName` User.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="bf323-118">**Note:** Requests with a `userId` or `userPrincipalName` are only accessible by the user or by a user with the User.ReadWrite.All permissions.</span></span> <span data-ttu-id="bf323-119">Para saber mais, confira [permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bf323-119">To learn more, see [Permissions](/graph/permissions-reference).</span></span>

## <a name="request-headers"></a><span data-ttu-id="bf323-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bf323-120">Request headers</span></span>

| <span data-ttu-id="bf323-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bf323-121">Header</span></span>       | <span data-ttu-id="bf323-122">Valor</span><span class="sxs-lookup"><span data-stu-id="bf323-122">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="bf323-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="bf323-123">Authorization</span></span>  | <span data-ttu-id="bf323-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bf323-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="bf323-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bf323-126">Content-Type</span></span>  | <span data-ttu-id="bf323-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bf323-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="bf323-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bf323-129">Request body</span></span>

<span data-ttu-id="bf323-p105">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="bf323-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="bf323-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bf323-133">Property</span></span>     | <span data-ttu-id="bf323-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="bf323-134">Type</span></span>   |<span data-ttu-id="bf323-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="bf323-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bf323-136">isEnabled</span><span class="sxs-lookup"><span data-stu-id="bf323-136">isEnabled</span></span>|<span data-ttu-id="bf323-137">Booliano</span><span class="sxs-lookup"><span data-stu-id="bf323-137">Boolean</span></span>| <span data-ttu-id="bf323-138">`true` se os insights **de item do usuárioInsights** e de horas de reunião estão habilitados; `false` se o item do **usuárioInights** e as percepções do horário de reunião estão desabilitados.</span><span class="sxs-lookup"><span data-stu-id="bf323-138">`true` if user's **itemInsights** and meeting hours insights are enabled; `false` if user's **itemInsights** and meeting hours insights are disabled.</span></span> <span data-ttu-id="bf323-139">O padrão é `true`.</span><span class="sxs-lookup"><span data-stu-id="bf323-139">Default is `true`.</span></span> <span data-ttu-id="bf323-140">Opcional.</span><span class="sxs-lookup"><span data-stu-id="bf323-140">Optional.</span></span>|

## <a name="response"></a><span data-ttu-id="bf323-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="bf323-141">Response</span></span>

<span data-ttu-id="bf323-142">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto userInsightsSettings](../resources/userinsightssettings.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bf323-142">If successful, this method returns a `200 OK` response code and [userInsightsSettings](../resources/userinsightssettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bf323-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bf323-143">Example</span></span> 

### <a name="request"></a><span data-ttu-id="bf323-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bf323-144">Request</span></span>

<span data-ttu-id="bf323-145">Veja a seguir uma solicitação de exemplo sobre como o usuário atualiza a configuração de privacidade "**isEnabled**" para desabilitar suas percepções de item e informações do horário de reunião.</span><span class="sxs-lookup"><span data-stu-id="bf323-145">The following is an example request on how user updates "**isEnabled**" privacy setting in order to disable his item insights and meeting hours insights.</span></span>

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


### <a name="response"></a><span data-ttu-id="bf323-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="bf323-146">Response</span></span>

<span data-ttu-id="bf323-147">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bf323-147">The following is an example of the response.</span></span> 

><span data-ttu-id="bf323-148">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="bf323-148">**Note:** The response object shown here might be shortened for readability.</span></span>
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
