---
title: Criar regra
description: 'Crie um objeto messageRule especificando um conjunto de condições e ações. '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 75acac9a8f8778ce7e2999960761d72bc5aa0309
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35454346"
---
# <a name="create-rule"></a><span data-ttu-id="1cb1c-103">Criar regra</span><span class="sxs-lookup"><span data-stu-id="1cb1c-103">Create rule</span></span>


<span data-ttu-id="1cb1c-104">Crie um objeto [messageRule](../resources/messagerule.md) especificando um conjunto de condições e ações.</span><span class="sxs-lookup"><span data-stu-id="1cb1c-104">Create a [messageRule](../resources/messagerule.md) object by specifying a set of conditions and actions.</span></span> 

<span data-ttu-id="1cb1c-105">O Outlook realizará essas ações se uma mensagem recebida na Caixa de Entrada do usuário atender às condições especificadas.</span><span class="sxs-lookup"><span data-stu-id="1cb1c-105">Outlook carries out those actions if an incoming message in the user's Inbox meets the specified conditions.</span></span>

## <a name="permissions"></a><span data-ttu-id="1cb1c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1cb1c-106">Permissions</span></span>
<span data-ttu-id="1cb1c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1cb1c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1cb1c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1cb1c-109">Permission type</span></span>      | <span data-ttu-id="1cb1c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1cb1c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1cb1c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1cb1c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1cb1c-112">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1cb1c-112">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="1cb1c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1cb1c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1cb1c-114">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1cb1c-114">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="1cb1c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1cb1c-115">Application</span></span> | <span data-ttu-id="1cb1c-116">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1cb1c-116">MailboxSettings.ReadWrite</span></span> |


## <a name="http-request"></a><span data-ttu-id="1cb1c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1cb1c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/mailFolders/inbox/messageRules
POST /users/{id | userPrincipalName}/mailFolders/inbox/messageRules
```
## <a name="request-headers"></a><span data-ttu-id="1cb1c-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1cb1c-118">Request headers</span></span>
| <span data-ttu-id="1cb1c-119">Nome</span><span class="sxs-lookup"><span data-stu-id="1cb1c-119">Name</span></span>       | <span data-ttu-id="1cb1c-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="1cb1c-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="1cb1c-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="1cb1c-121">Authorization</span></span>  | <span data-ttu-id="1cb1c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1cb1c-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="1cb1c-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1cb1c-124">Request body</span></span>
<span data-ttu-id="1cb1c-125">No corpo da solicitação, forneça os parâmetros que são aplicáveis à sua regra.</span><span class="sxs-lookup"><span data-stu-id="1cb1c-125">In the request body, supply the parameters that are applicable to your rule.</span></span> <span data-ttu-id="1cb1c-126">A seguir estão os parâmetros de corpo que normalmente são usados ao criar regras.</span><span class="sxs-lookup"><span data-stu-id="1cb1c-126">The following are body parameters that are typically used when creating rules.</span></span> <span data-ttu-id="1cb1c-127">É possível especificar outras propriedades **messageRule** graváveis conforme apropriado no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1cb1c-127">You can specify any other writable **messageRule** properties as appropriate in the request body.</span></span>

| <span data-ttu-id="1cb1c-128">Name</span><span class="sxs-lookup"><span data-stu-id="1cb1c-128">Name</span></span>       | <span data-ttu-id="1cb1c-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="1cb1c-129">Type</span></span>|<span data-ttu-id="1cb1c-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="1cb1c-130">Description</span></span>|
|:--------|:-------|:----------|
|<span data-ttu-id="1cb1c-131">actions</span><span class="sxs-lookup"><span data-stu-id="1cb1c-131">actions</span></span>|[<span data-ttu-id="1cb1c-132">messageRuleActions</span><span class="sxs-lookup"><span data-stu-id="1cb1c-132">messageRuleActions</span></span>](../resources/messageruleactions.md)|<span data-ttu-id="1cb1c-133">Ações a serem realizadas em uma mensagem quando as condições correspondentes, se houver, forem atendidas.</span><span class="sxs-lookup"><span data-stu-id="1cb1c-133">Actions to be taken on a message when the corresponding conditions, if any, are fulfilled.</span></span> <span data-ttu-id="1cb1c-134">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1cb1c-134">Required.</span></span>|
|<span data-ttu-id="1cb1c-135">conditions</span><span class="sxs-lookup"><span data-stu-id="1cb1c-135">conditions</span></span>|[<span data-ttu-id="1cb1c-136">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="1cb1c-136">messageRulePredicates</span></span>](../resources/messagerulepredicates.md)|<span data-ttu-id="1cb1c-137">Condições que, quando atendidas, acionarão as ações correspondentes dessa regra.</span><span class="sxs-lookup"><span data-stu-id="1cb1c-137">Conditions that when fulfilled, will trigger the corresponding actions for that rule.</span></span> <span data-ttu-id="1cb1c-138">Opcional.</span><span class="sxs-lookup"><span data-stu-id="1cb1c-138">Optional.</span></span>|
|<span data-ttu-id="1cb1c-139">displayName</span><span class="sxs-lookup"><span data-stu-id="1cb1c-139">displayName</span></span>| <span data-ttu-id="1cb1c-140">String</span><span class="sxs-lookup"><span data-stu-id="1cb1c-140">String</span></span>  | <span data-ttu-id="1cb1c-141">O nome de exibição da regra.</span><span class="sxs-lookup"><span data-stu-id="1cb1c-141">The display name of the rule.</span></span> <span data-ttu-id="1cb1c-142">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1cb1c-142">Required.</span></span>|
|<span data-ttu-id="1cb1c-143">exceptions</span><span class="sxs-lookup"><span data-stu-id="1cb1c-143">exceptions</span></span>| [<span data-ttu-id="1cb1c-144">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="1cb1c-144">messageRulePredicates</span></span>](../resources/messagerulepredicates.md)| <span data-ttu-id="1cb1c-145">Representa condições de exceção para a regra.</span><span class="sxs-lookup"><span data-stu-id="1cb1c-145">Represents exception conditions for the rule.</span></span> <span data-ttu-id="1cb1c-146">Opcional.</span><span class="sxs-lookup"><span data-stu-id="1cb1c-146">Optional.</span></span> |
|<span data-ttu-id="1cb1c-147">isEnabled</span><span class="sxs-lookup"><span data-stu-id="1cb1c-147">isEnabled</span></span> | <span data-ttu-id="1cb1c-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="1cb1c-148">Boolean</span></span> | <span data-ttu-id="1cb1c-149">Indica se a regra está habilitada para ser aplicada a mensagens.</span><span class="sxs-lookup"><span data-stu-id="1cb1c-149">Indicates whether the rule is enabled to be applied to messages.</span></span> <span data-ttu-id="1cb1c-150">Opcional.</span><span class="sxs-lookup"><span data-stu-id="1cb1c-150">Optional.</span></span> |
|<span data-ttu-id="1cb1c-151">sequence</span><span class="sxs-lookup"><span data-stu-id="1cb1c-151">sequence</span></span>| <span data-ttu-id="1cb1c-152">Int32</span><span class="sxs-lookup"><span data-stu-id="1cb1c-152">Int32</span></span> | <span data-ttu-id="1cb1c-153">Indica a ordem em que a regra é executada, entre outras regras.</span><span class="sxs-lookup"><span data-stu-id="1cb1c-153">Indicates the order in which the rule is executed, among other rules.</span></span> <span data-ttu-id="1cb1c-154">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1cb1c-154">Required.</span></span>|

## <a name="response"></a><span data-ttu-id="1cb1c-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="1cb1c-155">Response</span></span>
<span data-ttu-id="1cb1c-156">Se bem-sucedido, esse método retornará um código de resposta `201 Created` e um objeto **messageRule** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1cb1c-156">If successful, this method returns `201 Created` response code and a **messageRule** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1cb1c-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1cb1c-157">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1cb1c-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1cb1c-158">Request</span></span>
<span data-ttu-id="1cb1c-159">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1cb1c-159">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1cb1c-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="1cb1c-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["inbox"],
  "name": "create_messagerule_from_mailfolder"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messageRules
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="1cb1c-161">C#</span><span class="sxs-lookup"><span data-stu-id="1cb1c-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-messagerule-from-mailfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1cb1c-162">Javascript</span><span class="sxs-lookup"><span data-stu-id="1cb1c-162">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-messagerule-from-mailfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1cb1c-163">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="1cb1c-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-messagerule-from-mailfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="1cb1c-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="1cb1c-164">Response</span></span>
<span data-ttu-id="1cb1c-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1cb1c-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create rule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
