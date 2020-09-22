---
title: Criar regra
description: 'Crie um objeto messageRule especificando um conjunto de condições e ações. '
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 3851b34cf9e22b9e15501ce7ef3f9677ad7c5f64
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48027759"
---
# <a name="create-rule"></a><span data-ttu-id="3d339-103">Criar regra</span><span class="sxs-lookup"><span data-stu-id="3d339-103">Create rule</span></span>

<span data-ttu-id="3d339-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3d339-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3d339-105">Crie um objeto [messageRule](../resources/messagerule.md) especificando um conjunto de condições e ações.</span><span class="sxs-lookup"><span data-stu-id="3d339-105">Create a [messageRule](../resources/messagerule.md) object by specifying a set of conditions and actions.</span></span> 

<span data-ttu-id="3d339-106">O Outlook realizará essas ações se uma mensagem recebida na Caixa de Entrada do usuário atender às condições especificadas.</span><span class="sxs-lookup"><span data-stu-id="3d339-106">Outlook carries out those actions if an incoming message in the user's Inbox meets the specified conditions.</span></span>

## <a name="permissions"></a><span data-ttu-id="3d339-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="3d339-107">Permissions</span></span>
<span data-ttu-id="3d339-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3d339-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3d339-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3d339-110">Permission type</span></span>      | <span data-ttu-id="3d339-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3d339-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3d339-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3d339-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3d339-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3d339-113">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="3d339-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3d339-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3d339-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3d339-115">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="3d339-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3d339-116">Application</span></span> | <span data-ttu-id="3d339-117">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3d339-117">MailboxSettings.ReadWrite</span></span> |


## <a name="http-request"></a><span data-ttu-id="3d339-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3d339-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/mailFolders/inbox/messagerules
POST /users/{id | userPrincipalName}/mailFolders/inbox/messagerules
```
## <a name="request-headers"></a><span data-ttu-id="3d339-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3d339-119">Request headers</span></span>
| <span data-ttu-id="3d339-120">Nome</span><span class="sxs-lookup"><span data-stu-id="3d339-120">Name</span></span>       | <span data-ttu-id="3d339-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="3d339-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3d339-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="3d339-122">Authorization</span></span>  | <span data-ttu-id="3d339-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3d339-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="3d339-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3d339-125">Request body</span></span>
<span data-ttu-id="3d339-126">No corpo da solicitação, forneça os parâmetros que são aplicáveis à sua regra.</span><span class="sxs-lookup"><span data-stu-id="3d339-126">In the request body, supply the parameters that are applicable to your rule.</span></span> <span data-ttu-id="3d339-127">A seguir estão os parâmetros de corpo que normalmente são usados ao criar regras.</span><span class="sxs-lookup"><span data-stu-id="3d339-127">The following are body parameters that are typically used when creating rules.</span></span> <span data-ttu-id="3d339-128">É possível especificar outras propriedades **messageRule** graváveis conforme apropriado no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3d339-128">You can specify any other writable **messageRule** properties as appropriate in the request body.</span></span>

| <span data-ttu-id="3d339-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="3d339-129">Parameter</span></span>       | <span data-ttu-id="3d339-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="3d339-130">Type</span></span>|<span data-ttu-id="3d339-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="3d339-131">Description</span></span>|
|:--------|:-------|:----------|
|<span data-ttu-id="3d339-132">actions</span><span class="sxs-lookup"><span data-stu-id="3d339-132">actions</span></span>|[<span data-ttu-id="3d339-133">messageRuleActions</span><span class="sxs-lookup"><span data-stu-id="3d339-133">messageRuleActions</span></span>](../resources/messageruleactions.md)|<span data-ttu-id="3d339-134">Ações a serem realizadas em uma mensagem quando as condições correspondentes, se houver, forem atendidas.</span><span class="sxs-lookup"><span data-stu-id="3d339-134">Actions to be taken on a message when the corresponding conditions, if any, are fulfilled.</span></span> <span data-ttu-id="3d339-135">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3d339-135">Required.</span></span>|
|<span data-ttu-id="3d339-136">conditions</span><span class="sxs-lookup"><span data-stu-id="3d339-136">conditions</span></span>|[<span data-ttu-id="3d339-137">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="3d339-137">messageRulePredicates</span></span>](../resources/messagerulepredicates.md)|<span data-ttu-id="3d339-138">Condições que, quando atendidas, acionarão as ações correspondentes dessa regra.</span><span class="sxs-lookup"><span data-stu-id="3d339-138">Conditions that when fulfilled, will trigger the corresponding actions for that rule.</span></span> <span data-ttu-id="3d339-139">Opcional.</span><span class="sxs-lookup"><span data-stu-id="3d339-139">Optional.</span></span>|
|<span data-ttu-id="3d339-140">displayName</span><span class="sxs-lookup"><span data-stu-id="3d339-140">displayName</span></span>| <span data-ttu-id="3d339-141">String</span><span class="sxs-lookup"><span data-stu-id="3d339-141">String</span></span>  | <span data-ttu-id="3d339-142">O nome de exibição da regra.</span><span class="sxs-lookup"><span data-stu-id="3d339-142">The display name of the rule.</span></span> <span data-ttu-id="3d339-143">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3d339-143">Required.</span></span>|
|<span data-ttu-id="3d339-144">exceptions</span><span class="sxs-lookup"><span data-stu-id="3d339-144">exceptions</span></span>| [<span data-ttu-id="3d339-145">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="3d339-145">messageRulePredicates</span></span>](../resources/messagerulepredicates.md)| <span data-ttu-id="3d339-146">Representa condições de exceção para a regra.</span><span class="sxs-lookup"><span data-stu-id="3d339-146">Represents exception conditions for the rule.</span></span> <span data-ttu-id="3d339-147">Opcional.</span><span class="sxs-lookup"><span data-stu-id="3d339-147">Optional.</span></span> |
|<span data-ttu-id="3d339-148">isEnabled</span><span class="sxs-lookup"><span data-stu-id="3d339-148">isEnabled</span></span> | <span data-ttu-id="3d339-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="3d339-149">Boolean</span></span> | <span data-ttu-id="3d339-150">Indica se a regra está habilitada para ser aplicada a mensagens.</span><span class="sxs-lookup"><span data-stu-id="3d339-150">Indicates whether the rule is enabled to be applied to messages.</span></span> <span data-ttu-id="3d339-151">Opcional.</span><span class="sxs-lookup"><span data-stu-id="3d339-151">Optional.</span></span> |
|<span data-ttu-id="3d339-152">sequence</span><span class="sxs-lookup"><span data-stu-id="3d339-152">sequence</span></span>| <span data-ttu-id="3d339-153">Int32</span><span class="sxs-lookup"><span data-stu-id="3d339-153">Int32</span></span> | <span data-ttu-id="3d339-154">Indica a ordem em que a regra é executada, entre outras regras.</span><span class="sxs-lookup"><span data-stu-id="3d339-154">Indicates the order in which the rule is executed, among other rules.</span></span> <span data-ttu-id="3d339-155">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3d339-155">Required.</span></span>|

## <a name="response"></a><span data-ttu-id="3d339-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="3d339-156">Response</span></span>
<span data-ttu-id="3d339-157">Se bem-sucedido, esse método retornará um código de resposta `201 Created` e um objeto **messageRule** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3d339-157">If successful, this method returns `201 Created` response code and a **messageRule** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3d339-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3d339-158">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3d339-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3d339-159">Request</span></span>
<span data-ttu-id="3d339-160">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3d339-160">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3d339-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="3d339-161">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="3d339-162">C#</span><span class="sxs-lookup"><span data-stu-id="3d339-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-messagerule-from-mailfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3d339-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3d339-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-messagerule-from-mailfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3d339-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3d339-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-messagerule-from-mailfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="3d339-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="3d339-165">Response</span></span>
<span data-ttu-id="3d339-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3d339-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create rule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


