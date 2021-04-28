---
title: Atualizar regra
description: Altere as propriedades graváveis em um objeto messageRule e salve as alterações.
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 2b4aa70734a0dad302433f33b6f1ab2de888414a
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52039374"
---
# <a name="update-rule"></a><span data-ttu-id="2fac6-103">Atualizar regra</span><span class="sxs-lookup"><span data-stu-id="2fac6-103">Update rule</span></span>

<span data-ttu-id="2fac6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2fac6-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="2fac6-105">Altere as propriedades graváveis em um objeto [messageRule](../resources/messagerule.md) e salve as alterações.</span><span class="sxs-lookup"><span data-stu-id="2fac6-105">Change writable properties on a [messageRule](../resources/messagerule.md) object and save the changes.</span></span>

## <a name="permissions"></a><span data-ttu-id="2fac6-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="2fac6-106">Permissions</span></span>
<span data-ttu-id="2fac6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2fac6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2fac6-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2fac6-109">Permission type</span></span>      | <span data-ttu-id="2fac6-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2fac6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2fac6-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2fac6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2fac6-112">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2fac6-112">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="2fac6-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2fac6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2fac6-114">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2fac6-114">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="2fac6-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2fac6-115">Application</span></span> | <span data-ttu-id="2fac6-116">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2fac6-116">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="2fac6-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2fac6-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailFolders/inbox/messageRules/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/inbox/messageRules/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="2fac6-118">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="2fac6-118">Optional request headers</span></span>
| <span data-ttu-id="2fac6-119">Nome</span><span class="sxs-lookup"><span data-stu-id="2fac6-119">Name</span></span>       | <span data-ttu-id="2fac6-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="2fac6-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="2fac6-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="2fac6-121">Authorization</span></span>  | <span data-ttu-id="2fac6-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2fac6-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="2fac6-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2fac6-124">Request body</span></span>
<span data-ttu-id="2fac6-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="2fac6-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="2fac6-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2fac6-128">Property</span></span>     | <span data-ttu-id="2fac6-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="2fac6-129">Type</span></span>   |<span data-ttu-id="2fac6-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="2fac6-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2fac6-131">actions</span><span class="sxs-lookup"><span data-stu-id="2fac6-131">actions</span></span> | [<span data-ttu-id="2fac6-132">messageRuleActions</span><span class="sxs-lookup"><span data-stu-id="2fac6-132">messageRuleActions</span></span>](../resources/messageruleactions.md) | <span data-ttu-id="2fac6-133">Ações a serem realizadas em uma mensagem quando as condições correspondentes forem atendidas.</span><span class="sxs-lookup"><span data-stu-id="2fac6-133">Actions to be taken on a message when the corresponding conditions are fulfilled.</span></span> |
| <span data-ttu-id="2fac6-134">conditions</span><span class="sxs-lookup"><span data-stu-id="2fac6-134">conditions</span></span> | [<span data-ttu-id="2fac6-135">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="2fac6-135">messageRulePredicates</span></span>](../resources/messagerulepredicates.md) | <span data-ttu-id="2fac6-136">Condições que, quando atendidas, acionarão as ações correspondentes dessa regra.</span><span class="sxs-lookup"><span data-stu-id="2fac6-136">Conditions that when fulfilled, will trigger the corresponding actions for that rule.</span></span> |
| <span data-ttu-id="2fac6-137">displayName</span><span class="sxs-lookup"><span data-stu-id="2fac6-137">displayName</span></span> | <span data-ttu-id="2fac6-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2fac6-138">String</span></span> | <span data-ttu-id="2fac6-139">O nome de exibição da regra.</span><span class="sxs-lookup"><span data-stu-id="2fac6-139">The display name of the rule.</span></span> |
| <span data-ttu-id="2fac6-140">exceptions</span><span class="sxs-lookup"><span data-stu-id="2fac6-140">exceptions</span></span> | [<span data-ttu-id="2fac6-141">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="2fac6-141">messageRulePredicates</span></span>](../resources/messagerulepredicates.md) | <span data-ttu-id="2fac6-142">Condições de exceção para a regra.</span><span class="sxs-lookup"><span data-stu-id="2fac6-142">Exception conditions for the rule.</span></span> |
| <span data-ttu-id="2fac6-143">isEnabled</span><span class="sxs-lookup"><span data-stu-id="2fac6-143">isEnabled</span></span> | <span data-ttu-id="2fac6-144">Booliano</span><span class="sxs-lookup"><span data-stu-id="2fac6-144">Boolean</span></span> | <span data-ttu-id="2fac6-145">Indica se a regra está habilitada para ser aplicada a mensagens.</span><span class="sxs-lookup"><span data-stu-id="2fac6-145">Indicates whether the rule is enabled to be applied to messages.</span></span> |
| <span data-ttu-id="2fac6-146">isReadOnly</span><span class="sxs-lookup"><span data-stu-id="2fac6-146">isReadOnly</span></span> | <span data-ttu-id="2fac6-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="2fac6-147">Boolean</span></span> | <span data-ttu-id="2fac6-148">Indica se a regra é somente leitura e não pode ser modificada ou excluída pelas regras da API REST.</span><span class="sxs-lookup"><span data-stu-id="2fac6-148">Indicates if the rule is read-only and cannot be modified or deleted by the rules REST API.</span></span> |
| <span data-ttu-id="2fac6-149">sequence</span><span class="sxs-lookup"><span data-stu-id="2fac6-149">sequence</span></span> | <span data-ttu-id="2fac6-150">Int32</span><span class="sxs-lookup"><span data-stu-id="2fac6-150">Int32</span></span> | <span data-ttu-id="2fac6-151">Indica a ordem em que a regra é executada, entre outras regras.</span><span class="sxs-lookup"><span data-stu-id="2fac6-151">Indicates the order in which the rule is executed, among other rules.</span></span> |


## <a name="response"></a><span data-ttu-id="2fac6-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="2fac6-152">Response</span></span>
<span data-ttu-id="2fac6-153">Se tiver êxito, este método retornará um código de resposta `200 OK` e o objeto [messageRule](../resources/messagerule.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2fac6-153">If successful, this method returns a `200 OK` response code and updated [messageRule](../resources/messagerule.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2fac6-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2fac6-154">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2fac6-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2fac6-155">Request</span></span>
<span data-ttu-id="2fac6-156">O exemplo a seguir muda o nome da regra e as ações a serem seguidas para essa regra no [exemplo](messagerule-get.md#example) em [Obter regra](messagerule-get.md), do encaminhamento para um endereço a marcar sua importância como alta.</span><span class="sxs-lookup"><span data-stu-id="2fac6-156">The following example changes the name of the rule, and the actions to be taken for that rule in the [example](messagerule-get.md#example) in [Get rule](messagerule-get.md), from forwarding to an address to marking its importance as high.</span></span> 

# <a name="http"></a>[<span data-ttu-id="2fac6-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="2fac6-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["inbox", "AQAAAJ5dZqA="],
  "name": "update_messagerule"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messageRules/AQAAAJ5dZqA=
Content-type: application/json

{
    "displayName": "Important from partner",
    "actions": {
        "markImportance": "high"
     }
} 
```
# <a name="c"></a>[<span data-ttu-id="2fac6-158">C#</span><span class="sxs-lookup"><span data-stu-id="2fac6-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-messagerule-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2fac6-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2fac6-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-messagerule-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2fac6-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2fac6-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-messagerule-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2fac6-161">Java</span><span class="sxs-lookup"><span data-stu-id="2fac6-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-messagerule-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="2fac6-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="2fac6-162">Response</span></span>
<span data-ttu-id="2fac6-163">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2fac6-163">Here is an example of the response.</span></span> <span data-ttu-id="2fac6-164">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="2fac6-164">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.messageRule"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Me/mailFolders('inbox')/messageRules/$entity",
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
<!-- {
  "type": "#page.annotation",
  "description": "Update rule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

