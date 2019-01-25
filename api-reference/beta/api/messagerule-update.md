---
title: Atualizar regra
description: Altere as propriedades graváveis em um objeto messageRule e salve as alterações.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 97ef83d1e4085b8eb8c47d90c750c86232a314f1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519623"
---
# <a name="update-rule"></a><span data-ttu-id="eeb01-103">Atualizar regra</span><span class="sxs-lookup"><span data-stu-id="eeb01-103">Update rule</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eeb01-104">Altere as propriedades graváveis em um objeto [messageRule](../resources/messagerule.md) e salve as alterações.</span><span class="sxs-lookup"><span data-stu-id="eeb01-104">Change writable properties on a [messageRule](../resources/messagerule.md) object and save the changes.</span></span>

## <a name="permissions"></a><span data-ttu-id="eeb01-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="eeb01-105">Permissions</span></span>
<span data-ttu-id="eeb01-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eeb01-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eeb01-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eeb01-108">Permission type</span></span>      | <span data-ttu-id="eeb01-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="eeb01-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eeb01-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eeb01-110">Delegated (work or school account)</span></span> | <span data-ttu-id="eeb01-111">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eeb01-111">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="eeb01-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eeb01-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eeb01-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eeb01-113">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="eeb01-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eeb01-114">Application</span></span> | <span data-ttu-id="eeb01-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eeb01-115">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="eeb01-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eeb01-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailFolders/inbox/messagerules/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/inbox/messagerules/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="eeb01-117">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="eeb01-117">Optional request headers</span></span>
| <span data-ttu-id="eeb01-118">Nome</span><span class="sxs-lookup"><span data-stu-id="eeb01-118">Name</span></span>       | <span data-ttu-id="eeb01-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="eeb01-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="eeb01-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="eeb01-120">Authorization</span></span>  | <span data-ttu-id="eeb01-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eeb01-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="eeb01-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eeb01-123">Request body</span></span>
<span data-ttu-id="eeb01-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="eeb01-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="eeb01-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eeb01-127">Property</span></span>     | <span data-ttu-id="eeb01-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="eeb01-128">Type</span></span>   |<span data-ttu-id="eeb01-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="eeb01-129">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="eeb01-130">actions</span><span class="sxs-lookup"><span data-stu-id="eeb01-130">actions</span></span> | [<span data-ttu-id="eeb01-131">messageRuleActions</span><span class="sxs-lookup"><span data-stu-id="eeb01-131">messageRuleActions</span></span>](../resources/messageruleactions.md) | <span data-ttu-id="eeb01-132">Ações a serem realizadas em uma mensagem quando as condições correspondentes forem atendidas.</span><span class="sxs-lookup"><span data-stu-id="eeb01-132">Actions to be taken on a message when the corresponding conditions are fulfilled.</span></span> |
| <span data-ttu-id="eeb01-133">conditions</span><span class="sxs-lookup"><span data-stu-id="eeb01-133">conditions</span></span> | [<span data-ttu-id="eeb01-134">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="eeb01-134">messageRulePredicates</span></span>](../resources/messagerulepredicates.md) | <span data-ttu-id="eeb01-135">Condições que, quando atendidas, acionarão as ações correspondentes dessa regra.</span><span class="sxs-lookup"><span data-stu-id="eeb01-135">Conditions that when fulfilled, will trigger the corresponding actions for that rule.</span></span> |
| <span data-ttu-id="eeb01-136">displayName</span><span class="sxs-lookup"><span data-stu-id="eeb01-136">displayName</span></span> | <span data-ttu-id="eeb01-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="eeb01-137">String</span></span> | <span data-ttu-id="eeb01-138">O nome de exibição da regra.</span><span class="sxs-lookup"><span data-stu-id="eeb01-138">The display name of the rule.</span></span> |
| <span data-ttu-id="eeb01-139">exceptions</span><span class="sxs-lookup"><span data-stu-id="eeb01-139">exceptions</span></span> | [<span data-ttu-id="eeb01-140">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="eeb01-140">messageRulePredicates</span></span>](../resources/messagerulepredicates.md) | <span data-ttu-id="eeb01-141">Condições de exceção para a regra.</span><span class="sxs-lookup"><span data-stu-id="eeb01-141">Exception conditions for the rule.</span></span> |
| <span data-ttu-id="eeb01-142">isEnabled</span><span class="sxs-lookup"><span data-stu-id="eeb01-142">isEnabled</span></span> | <span data-ttu-id="eeb01-143">Booliano</span><span class="sxs-lookup"><span data-stu-id="eeb01-143">Boolean</span></span> | <span data-ttu-id="eeb01-144">Indica se a regra está habilitada para ser aplicada a mensagens.</span><span class="sxs-lookup"><span data-stu-id="eeb01-144">Indicates whether the rule is enabled to be applied to messages.</span></span> |
| <span data-ttu-id="eeb01-145">isReadOnly</span><span class="sxs-lookup"><span data-stu-id="eeb01-145">isReadOnly</span></span> | <span data-ttu-id="eeb01-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="eeb01-146">Boolean</span></span> | <span data-ttu-id="eeb01-147">Indica se a regra é somente leitura e não pode ser modificada ou excluída pelas regras da API REST.</span><span class="sxs-lookup"><span data-stu-id="eeb01-147">Indicates if the rule is read-only and cannot be modified or deleted by the rules REST API.</span></span> |
| <span data-ttu-id="eeb01-148">sequence</span><span class="sxs-lookup"><span data-stu-id="eeb01-148">sequence</span></span> | <span data-ttu-id="eeb01-149">Int32</span><span class="sxs-lookup"><span data-stu-id="eeb01-149">Int32</span></span> | <span data-ttu-id="eeb01-150">Indica a ordem em que a regra é executada, entre outras regras.</span><span class="sxs-lookup"><span data-stu-id="eeb01-150">Indicates the order in which the rule is executed, among other rules.</span></span> |


## <a name="response"></a><span data-ttu-id="eeb01-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="eeb01-151">Response</span></span>
<span data-ttu-id="eeb01-152">Se tiver êxito, este método retornará um código de resposta `200 OK` e o objeto [messageRule](../resources/messagerule.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eeb01-152">If successful, this method returns a `200 OK` response code and updated [messageRule](../resources/messagerule.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="eeb01-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eeb01-153">Example</span></span>
##### <a name="request"></a><span data-ttu-id="eeb01-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eeb01-154">Request</span></span>
<span data-ttu-id="eeb01-155">O exemplo a seguir muda o nome da regra e as ações a serem seguidas para essa regra no [exemplo](messagerule-get.md#example) em [Obter regra](messagerule-get.md), do encaminhamento para um endereço a marcar sua importância como alta.</span><span class="sxs-lookup"><span data-stu-id="eeb01-155">The following example changes the name of the rule, and the actions to be taken for that rule in the [example](messagerule-get.md#example) in [Get rule](messagerule-get.md), from forwarding to an address to marking its importance as high.</span></span> 
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
##### <a name="response"></a><span data-ttu-id="eeb01-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="eeb01-156">Response</span></span>
<span data-ttu-id="eeb01-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="eeb01-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/messagerule-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
