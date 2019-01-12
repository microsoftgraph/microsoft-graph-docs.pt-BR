---
title: Atualizar regra
description: Altere as propriedades graváveis em um objeto messageRule e salve as alterações.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: ce58fd5c3a1156273cec9c62f322d4fe198d03f7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27919896"
---
# <a name="update-rule"></a><span data-ttu-id="eaa11-103">Atualizar regra</span><span class="sxs-lookup"><span data-stu-id="eaa11-103">Update rule</span></span>

> <span data-ttu-id="eaa11-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="eaa11-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="eaa11-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="eaa11-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="eaa11-106">Altere as propriedades graváveis em um objeto [messageRule](../resources/messagerule.md) e salve as alterações.</span><span class="sxs-lookup"><span data-stu-id="eaa11-106">Change writable properties on a [messageRule](../resources/messagerule.md) object and save the changes.</span></span>

## <a name="permissions"></a><span data-ttu-id="eaa11-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="eaa11-107">Permissions</span></span>
<span data-ttu-id="eaa11-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eaa11-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eaa11-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eaa11-110">Permission type</span></span>      | <span data-ttu-id="eaa11-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="eaa11-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eaa11-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eaa11-112">Delegated (work or school account)</span></span> | <span data-ttu-id="eaa11-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eaa11-113">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="eaa11-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eaa11-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eaa11-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eaa11-115">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="eaa11-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eaa11-116">Application</span></span> | <span data-ttu-id="eaa11-117">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eaa11-117">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="eaa11-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eaa11-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailFolders/inbox/messagerules/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/inbox/messagerules/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="eaa11-119">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="eaa11-119">Optional request headers</span></span>
| <span data-ttu-id="eaa11-120">Nome</span><span class="sxs-lookup"><span data-stu-id="eaa11-120">Name</span></span>       | <span data-ttu-id="eaa11-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="eaa11-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="eaa11-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="eaa11-122">Authorization</span></span>  | <span data-ttu-id="eaa11-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eaa11-p103">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="eaa11-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eaa11-125">Request body</span></span>
<span data-ttu-id="eaa11-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="eaa11-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="eaa11-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eaa11-129">Property</span></span>     | <span data-ttu-id="eaa11-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="eaa11-130">Type</span></span>   |<span data-ttu-id="eaa11-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="eaa11-131">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="eaa11-132">actions</span><span class="sxs-lookup"><span data-stu-id="eaa11-132">actions</span></span> | [<span data-ttu-id="eaa11-133">messageRuleActions</span><span class="sxs-lookup"><span data-stu-id="eaa11-133">messageRuleActions</span></span>](../resources/messageruleactions.md) | <span data-ttu-id="eaa11-134">Ações a serem realizadas em uma mensagem quando as condições correspondentes forem atendidas.</span><span class="sxs-lookup"><span data-stu-id="eaa11-134">Actions to be taken on a message when the corresponding conditions are fulfilled.</span></span> |
| <span data-ttu-id="eaa11-135">conditions</span><span class="sxs-lookup"><span data-stu-id="eaa11-135">conditions</span></span> | [<span data-ttu-id="eaa11-136">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="eaa11-136">messageRulePredicates</span></span>](../resources/messagerulepredicates.md) | <span data-ttu-id="eaa11-137">Condições que, quando atendidas, acionarão as ações correspondentes dessa regra.</span><span class="sxs-lookup"><span data-stu-id="eaa11-137">Conditions that when fulfilled, will trigger the corresponding actions for that rule.</span></span> |
| <span data-ttu-id="eaa11-138">displayName</span><span class="sxs-lookup"><span data-stu-id="eaa11-138">displayName</span></span> | <span data-ttu-id="eaa11-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="eaa11-139">String</span></span> | <span data-ttu-id="eaa11-140">O nome de exibição da regra.</span><span class="sxs-lookup"><span data-stu-id="eaa11-140">The display name of the rule.</span></span> |
| <span data-ttu-id="eaa11-141">exceptions</span><span class="sxs-lookup"><span data-stu-id="eaa11-141">exceptions</span></span> | [<span data-ttu-id="eaa11-142">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="eaa11-142">messageRulePredicates</span></span>](../resources/messagerulepredicates.md) | <span data-ttu-id="eaa11-143">Condições de exceção para a regra.</span><span class="sxs-lookup"><span data-stu-id="eaa11-143">Exception conditions for the rule.</span></span> |
| <span data-ttu-id="eaa11-144">isEnabled</span><span class="sxs-lookup"><span data-stu-id="eaa11-144">isEnabled</span></span> | <span data-ttu-id="eaa11-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="eaa11-145">Boolean</span></span> | <span data-ttu-id="eaa11-146">Indica se a regra está habilitada para ser aplicada a mensagens.</span><span class="sxs-lookup"><span data-stu-id="eaa11-146">Indicates whether the rule is enabled to be applied to messages.</span></span> |
| <span data-ttu-id="eaa11-147">isReadOnly</span><span class="sxs-lookup"><span data-stu-id="eaa11-147">isReadOnly</span></span> | <span data-ttu-id="eaa11-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="eaa11-148">Boolean</span></span> | <span data-ttu-id="eaa11-149">Indica se a regra é somente leitura e não pode ser modificada ou excluída pelas regras da API REST.</span><span class="sxs-lookup"><span data-stu-id="eaa11-149">Indicates if the rule is read-only and cannot be modified or deleted by the rules REST API.</span></span> |
| <span data-ttu-id="eaa11-150">sequence</span><span class="sxs-lookup"><span data-stu-id="eaa11-150">sequence</span></span> | <span data-ttu-id="eaa11-151">Int32</span><span class="sxs-lookup"><span data-stu-id="eaa11-151">Int32</span></span> | <span data-ttu-id="eaa11-152">Indica a ordem em que a regra é executada, entre outras regras.</span><span class="sxs-lookup"><span data-stu-id="eaa11-152">Indicates the order in which the rule is executed, among other rules.</span></span> |


## <a name="response"></a><span data-ttu-id="eaa11-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="eaa11-153">Response</span></span>
<span data-ttu-id="eaa11-154">Se tiver êxito, este método retornará um código de resposta `200 OK` e o objeto [messageRule](../resources/messagerule.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eaa11-154">If successful, this method returns a `200 OK` response code and updated [messageRule](../resources/messagerule.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="eaa11-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eaa11-155">Example</span></span>
##### <a name="request"></a><span data-ttu-id="eaa11-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eaa11-156">Request</span></span>
<span data-ttu-id="eaa11-157">O exemplo a seguir muda o nome da regra e as ações a serem seguidas para essa regra no [exemplo](messagerule-get.md#example) em [Obter regra](messagerule-get.md), do encaminhamento para um endereço a marcar sua importância como alta.</span><span class="sxs-lookup"><span data-stu-id="eaa11-157">The following example changes the name of the rule, and the actions to be taken for that rule in the [example](messagerule-get.md#example) in [Get rule](messagerule-get.md), from forwarding to an address to marking its importance as high.</span></span> 
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
##### <a name="response"></a><span data-ttu-id="eaa11-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="eaa11-158">Response</span></span>
<span data-ttu-id="eaa11-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="eaa11-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Update rule",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
