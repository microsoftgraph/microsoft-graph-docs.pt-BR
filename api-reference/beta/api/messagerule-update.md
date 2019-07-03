---
title: Atualizar regra
description: Altere as propriedades graváveis em um objeto messageRule e salve as alterações.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: b6371057d92fddaecfb5c26aad70054114749ab3
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35447904"
---
# <a name="update-rule"></a><span data-ttu-id="bf478-103">Atualizar regra</span><span class="sxs-lookup"><span data-stu-id="bf478-103">Update rule</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bf478-104">Altere as propriedades graváveis em um objeto [messageRule](../resources/messagerule.md) e salve as alterações.</span><span class="sxs-lookup"><span data-stu-id="bf478-104">Change writable properties on a [messageRule](../resources/messagerule.md) object and save the changes.</span></span>

## <a name="permissions"></a><span data-ttu-id="bf478-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="bf478-105">Permissions</span></span>
<span data-ttu-id="bf478-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bf478-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bf478-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bf478-108">Permission type</span></span>      | <span data-ttu-id="bf478-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bf478-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bf478-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bf478-110">Delegated (work or school account)</span></span> | <span data-ttu-id="bf478-111">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bf478-111">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="bf478-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bf478-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bf478-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bf478-113">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="bf478-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bf478-114">Application</span></span> | <span data-ttu-id="bf478-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bf478-115">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="bf478-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bf478-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailFolders/inbox/messagerules/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/inbox/messagerules/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="bf478-117">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="bf478-117">Optional request headers</span></span>
| <span data-ttu-id="bf478-118">Nome</span><span class="sxs-lookup"><span data-stu-id="bf478-118">Name</span></span>       | <span data-ttu-id="bf478-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="bf478-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="bf478-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="bf478-120">Authorization</span></span>  | <span data-ttu-id="bf478-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bf478-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="bf478-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bf478-123">Request body</span></span>
<span data-ttu-id="bf478-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="bf478-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="bf478-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bf478-127">Property</span></span>     | <span data-ttu-id="bf478-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="bf478-128">Type</span></span>   |<span data-ttu-id="bf478-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="bf478-129">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="bf478-130">actions</span><span class="sxs-lookup"><span data-stu-id="bf478-130">actions</span></span> | [<span data-ttu-id="bf478-131">messageRuleActions</span><span class="sxs-lookup"><span data-stu-id="bf478-131">messageRuleActions</span></span>](../resources/messageruleactions.md) | <span data-ttu-id="bf478-132">Ações a serem realizadas em uma mensagem quando as condições correspondentes forem atendidas.</span><span class="sxs-lookup"><span data-stu-id="bf478-132">Actions to be taken on a message when the corresponding conditions are fulfilled.</span></span> |
| <span data-ttu-id="bf478-133">conditions</span><span class="sxs-lookup"><span data-stu-id="bf478-133">conditions</span></span> | [<span data-ttu-id="bf478-134">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="bf478-134">messageRulePredicates</span></span>](../resources/messagerulepredicates.md) | <span data-ttu-id="bf478-135">Condições que, quando atendidas, acionarão as ações correspondentes dessa regra.</span><span class="sxs-lookup"><span data-stu-id="bf478-135">Conditions that when fulfilled, will trigger the corresponding actions for that rule.</span></span> |
| <span data-ttu-id="bf478-136">displayName</span><span class="sxs-lookup"><span data-stu-id="bf478-136">displayName</span></span> | <span data-ttu-id="bf478-137">String</span><span class="sxs-lookup"><span data-stu-id="bf478-137">String</span></span> | <span data-ttu-id="bf478-138">O nome de exibição da regra.</span><span class="sxs-lookup"><span data-stu-id="bf478-138">The display name of the rule.</span></span> |
| <span data-ttu-id="bf478-139">exceptions</span><span class="sxs-lookup"><span data-stu-id="bf478-139">exceptions</span></span> | [<span data-ttu-id="bf478-140">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="bf478-140">messageRulePredicates</span></span>](../resources/messagerulepredicates.md) | <span data-ttu-id="bf478-141">Condições de exceção para a regra.</span><span class="sxs-lookup"><span data-stu-id="bf478-141">Exception conditions for the rule.</span></span> |
| <span data-ttu-id="bf478-142">isEnabled</span><span class="sxs-lookup"><span data-stu-id="bf478-142">isEnabled</span></span> | <span data-ttu-id="bf478-143">Booliano</span><span class="sxs-lookup"><span data-stu-id="bf478-143">Boolean</span></span> | <span data-ttu-id="bf478-144">Indica se a regra está habilitada para ser aplicada a mensagens.</span><span class="sxs-lookup"><span data-stu-id="bf478-144">Indicates whether the rule is enabled to be applied to messages.</span></span> |
| <span data-ttu-id="bf478-145">isReadOnly</span><span class="sxs-lookup"><span data-stu-id="bf478-145">isReadOnly</span></span> | <span data-ttu-id="bf478-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf478-146">Boolean</span></span> | <span data-ttu-id="bf478-147">Indica se a regra é somente leitura e não pode ser modificada ou excluída pelas regras da API REST.</span><span class="sxs-lookup"><span data-stu-id="bf478-147">Indicates if the rule is read-only and cannot be modified or deleted by the rules REST API.</span></span> |
| <span data-ttu-id="bf478-148">sequence</span><span class="sxs-lookup"><span data-stu-id="bf478-148">sequence</span></span> | <span data-ttu-id="bf478-149">Int32</span><span class="sxs-lookup"><span data-stu-id="bf478-149">Int32</span></span> | <span data-ttu-id="bf478-150">Indica a ordem em que a regra é executada, entre outras regras.</span><span class="sxs-lookup"><span data-stu-id="bf478-150">Indicates the order in which the rule is executed, among other rules.</span></span> |


## <a name="response"></a><span data-ttu-id="bf478-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="bf478-151">Response</span></span>
<span data-ttu-id="bf478-152">Se tiver êxito, este método retornará um código de resposta `200 OK` e o objeto [messageRule](../resources/messagerule.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bf478-152">If successful, this method returns a `200 OK` response code and updated [messageRule](../resources/messagerule.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bf478-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bf478-153">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bf478-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bf478-154">Request</span></span>
<span data-ttu-id="bf478-155">O exemplo a seguir muda o nome da regra e as ações a serem seguidas para essa regra no [exemplo](messagerule-get.md#example) em [Obter regra](messagerule-get.md), do encaminhamento para um endereço a marcar sua importância como alta.</span><span class="sxs-lookup"><span data-stu-id="bf478-155">The following example changes the name of the rule, and the actions to be taken for that rule in the [example](messagerule-get.md#example) in [Get rule](messagerule-get.md), from forwarding to an address to marking its importance as high.</span></span> 

# <a name="httptabhttp"></a>[<span data-ttu-id="bf478-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="bf478-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_messagerule"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/mailfolders/inbox/messagerules('AQAAAJ5dZqA=')
Content-type: application/json

{
    "displayName": "Important from partner",
    "actions": {
        "markImportance": "high"
     }
} 
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="bf478-157">C#</span><span class="sxs-lookup"><span data-stu-id="bf478-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-messagerule-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bf478-158">Javascript</span><span class="sxs-lookup"><span data-stu-id="bf478-158">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-messagerule-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="bf478-159">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="bf478-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-messagerule-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="bf478-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="bf478-160">Response</span></span>
<span data-ttu-id="bf478-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bf478-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.messageRule"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#Me/mailFolders('inbox')/messageRules/$entity",
  "id":"AQAAAJ5dZqA=",
  "displayName":"Important from partner",
  "sequence":2,
  "isEnabled":true,
  "hasError":false,
  "isReadOnly":false,
  "conditions":{
    "senderContains":[
      "ADELE"
    ]
  },
  "actions":{
    "markImportance": "high"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update rule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
