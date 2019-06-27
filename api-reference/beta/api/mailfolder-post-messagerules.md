---
title: Criar regra
description: 'Crie um objeto messageRule especificando um conjunto de condições e ações. '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 2d42db335a8e08e813081b51c9ffdd055cb8860a
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35266651"
---
# <a name="create-rule"></a><span data-ttu-id="e31ee-103">Criar regra</span><span class="sxs-lookup"><span data-stu-id="e31ee-103">Create rule</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e31ee-104">Crie um objeto [messageRule](../resources/messagerule.md) especificando um conjunto de condições e ações.</span><span class="sxs-lookup"><span data-stu-id="e31ee-104">Create a [messageRule](../resources/messagerule.md) object by specifying a set of conditions and actions.</span></span> 

<span data-ttu-id="e31ee-105">O Outlook realizará essas ações se uma mensagem recebida na Caixa de Entrada do usuário atender às condições especificadas.</span><span class="sxs-lookup"><span data-stu-id="e31ee-105">Outlook carries out those actions if an incoming message in the user's Inbox meets the specified conditions.</span></span>

## <a name="permissions"></a><span data-ttu-id="e31ee-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e31ee-106">Permissions</span></span>
<span data-ttu-id="e31ee-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e31ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e31ee-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e31ee-109">Permission type</span></span>      | <span data-ttu-id="e31ee-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e31ee-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e31ee-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e31ee-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e31ee-112">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e31ee-112">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="e31ee-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e31ee-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e31ee-114">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e31ee-114">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="e31ee-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e31ee-115">Application</span></span> | <span data-ttu-id="e31ee-116">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e31ee-116">MailboxSettings.ReadWrite</span></span> |


## <a name="http-request"></a><span data-ttu-id="e31ee-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e31ee-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/mailFolders/inbox/messagerules
POST /users/{id | userPrincipalName}/mailFolders/inbox/messagerules
```
## <a name="request-headers"></a><span data-ttu-id="e31ee-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e31ee-118">Request headers</span></span>
| <span data-ttu-id="e31ee-119">Nome</span><span class="sxs-lookup"><span data-stu-id="e31ee-119">Name</span></span>       | <span data-ttu-id="e31ee-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="e31ee-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e31ee-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="e31ee-121">Authorization</span></span>  | <span data-ttu-id="e31ee-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e31ee-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="e31ee-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e31ee-124">Request body</span></span>
<span data-ttu-id="e31ee-125">No corpo da solicitação, forneça os parâmetros que são aplicáveis à sua regra.</span><span class="sxs-lookup"><span data-stu-id="e31ee-125">In the request body, supply the parameters that are applicable to your rule.</span></span> <span data-ttu-id="e31ee-126">A seguir estão os parâmetros de corpo que normalmente são usados ao criar regras.</span><span class="sxs-lookup"><span data-stu-id="e31ee-126">The following are body parameters that are typically used when creating rules.</span></span> <span data-ttu-id="e31ee-127">É possível especificar outras propriedades **messageRule** graváveis conforme apropriado no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e31ee-127">You can specify any other writable **messageRule** properties as appropriate in the request body.</span></span>

| <span data-ttu-id="e31ee-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="e31ee-128">Parameter</span></span>       | <span data-ttu-id="e31ee-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="e31ee-129">Type</span></span>|<span data-ttu-id="e31ee-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="e31ee-130">Description</span></span>|
|:--------|:-------|:----------|
|<span data-ttu-id="e31ee-131">actions</span><span class="sxs-lookup"><span data-stu-id="e31ee-131">actions</span></span>|[<span data-ttu-id="e31ee-132">messageRuleActions</span><span class="sxs-lookup"><span data-stu-id="e31ee-132">messageRuleActions</span></span>](../resources/messageruleactions.md)|<span data-ttu-id="e31ee-133">Ações a serem realizadas em uma mensagem quando as condições correspondentes, se houver, forem atendidas.</span><span class="sxs-lookup"><span data-stu-id="e31ee-133">Actions to be taken on a message when the corresponding conditions, if any, are fulfilled.</span></span> <span data-ttu-id="e31ee-134">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e31ee-134">Required.</span></span>|
|<span data-ttu-id="e31ee-135">conditions</span><span class="sxs-lookup"><span data-stu-id="e31ee-135">conditions</span></span>|[<span data-ttu-id="e31ee-136">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="e31ee-136">messageRulePredicates</span></span>](../resources/messagerulepredicates.md)|<span data-ttu-id="e31ee-137">Condições que, quando atendidas, acionarão as ações correspondentes dessa regra.</span><span class="sxs-lookup"><span data-stu-id="e31ee-137">Conditions that when fulfilled, will trigger the corresponding actions for that rule.</span></span> <span data-ttu-id="e31ee-138">Opcional.</span><span class="sxs-lookup"><span data-stu-id="e31ee-138">Optional.</span></span>|
|<span data-ttu-id="e31ee-139">displayName</span><span class="sxs-lookup"><span data-stu-id="e31ee-139">displayName</span></span>| <span data-ttu-id="e31ee-140">String</span><span class="sxs-lookup"><span data-stu-id="e31ee-140">String</span></span>  | <span data-ttu-id="e31ee-141">O nome de exibição da regra.</span><span class="sxs-lookup"><span data-stu-id="e31ee-141">The display name of the rule.</span></span> <span data-ttu-id="e31ee-142">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e31ee-142">Required.</span></span>|
|<span data-ttu-id="e31ee-143">exceptions</span><span class="sxs-lookup"><span data-stu-id="e31ee-143">exceptions</span></span>| [<span data-ttu-id="e31ee-144">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="e31ee-144">messageRulePredicates</span></span>](../resources/messagerulepredicates.md)| <span data-ttu-id="e31ee-145">Representa condições de exceção para a regra.</span><span class="sxs-lookup"><span data-stu-id="e31ee-145">Represents exception conditions for the rule.</span></span> <span data-ttu-id="e31ee-146">Opcional.</span><span class="sxs-lookup"><span data-stu-id="e31ee-146">Optional.</span></span> |
|<span data-ttu-id="e31ee-147">isEnabled</span><span class="sxs-lookup"><span data-stu-id="e31ee-147">isEnabled</span></span> | <span data-ttu-id="e31ee-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="e31ee-148">Boolean</span></span> | <span data-ttu-id="e31ee-149">Indica se a regra está habilitada para ser aplicada a mensagens.</span><span class="sxs-lookup"><span data-stu-id="e31ee-149">Indicates whether the rule is enabled to be applied to messages.</span></span> <span data-ttu-id="e31ee-150">Opcional.</span><span class="sxs-lookup"><span data-stu-id="e31ee-150">Optional.</span></span> |
|<span data-ttu-id="e31ee-151">sequence</span><span class="sxs-lookup"><span data-stu-id="e31ee-151">sequence</span></span>| <span data-ttu-id="e31ee-152">Int32</span><span class="sxs-lookup"><span data-stu-id="e31ee-152">Int32</span></span> | <span data-ttu-id="e31ee-153">Indica a ordem em que a regra é executada, entre outras regras.</span><span class="sxs-lookup"><span data-stu-id="e31ee-153">Indicates the order in which the rule is executed, among other rules.</span></span> <span data-ttu-id="e31ee-154">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e31ee-154">Required.</span></span>|

## <a name="response"></a><span data-ttu-id="e31ee-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="e31ee-155">Response</span></span>
<span data-ttu-id="e31ee-156">Se bem-sucedido, esse método retornará um código de resposta `201 Created` e um objeto **messageRule** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e31ee-156">If successful, this method returns `201 Created` response code and a **messageRule** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e31ee-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e31ee-157">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e31ee-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e31ee-158">Request</span></span>
<span data-ttu-id="e31ee-159">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e31ee-159">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_messagerule_from_mailfolder"
}-->
```http
POST https://graph.microsoft.com/beta/me/mailFolders/inbox/messagerules
Content-type: application/json

{      
    "displayName": "From partner",      
    "sequence": 2,      
    "isEnabled": true,          
    "conditions": {
        "senderContains": [
          "adele"       
        ]
     },
     "actions": {
        "forwardTo": [
          {
             "emailAddress": {
                "name": "Alex Wilbur",
                "address": "AlexW@contoso.onmicrosoft.com"
              }
           }
        ],
        "stopProcessingRules": true
     }    
}

```
##### <a name="response"></a><span data-ttu-id="e31ee-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="e31ee-160">Response</span></span>
<span data-ttu-id="e31ee-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e31ee-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.messageRule"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id":"AQAAAJ5dZqA=",
  "displayName":"From partner",
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
      "stopProcessingRules":true,
      "forwardTo":[
        {
          "emailAddress":{
            "name":"Alex Wilbur",
            "address":"AlexW@contoso.onmicrosoft.com"
          }
        }
      ]
  }
}

```
#### <a name="sdk-sample-code"></a><span data-ttu-id="e31ee-164">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="e31ee-164">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e31ee-165">C#</span><span class="sxs-lookup"><span data-stu-id="e31ee-165">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_messagerule_from_mailfolder-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e31ee-166">Javascript</span><span class="sxs-lookup"><span data-stu-id="e31ee-166">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_messagerule_from_mailfolder-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="e31ee-167">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="e31ee-167">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_messagerule_from_mailfolder-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create rule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/mailfolder-post-messagerules.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/mailfolder-post-messagerules.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/mailfolder-post-messagerules.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
