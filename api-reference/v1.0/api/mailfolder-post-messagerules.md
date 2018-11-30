---
title: Criar regra
description: 'Crie um objeto messageRule especificando um conjunto de condições e ações. '
ms.openlocfilehash: fdea3920e272581c8d08e04c01c385575e6c6df1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005213"
---
# <a name="create-rule"></a><span data-ttu-id="63aa4-103">Criar regra</span><span class="sxs-lookup"><span data-stu-id="63aa4-103">Create rule</span></span>


<span data-ttu-id="63aa4-104">Crie um objeto [messageRule](../resources/messagerule.md) especificando um conjunto de condições e ações.</span><span class="sxs-lookup"><span data-stu-id="63aa4-104">Create a [messageRule](../resources/messagerule.md) object by specifying a set of conditions and actions.</span></span> 

<span data-ttu-id="63aa4-105">O Outlook realizará essas ações se uma mensagem recebida na Caixa de Entrada do usuário atender às condições especificadas.</span><span class="sxs-lookup"><span data-stu-id="63aa4-105">Outlook carries out those actions if an incoming message in the user's Inbox meets the specified conditions.</span></span>

## <a name="permissions"></a><span data-ttu-id="63aa4-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="63aa4-106">Permissions</span></span>
<span data-ttu-id="63aa4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="63aa4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="63aa4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="63aa4-109">Permission type</span></span>      | <span data-ttu-id="63aa4-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="63aa4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="63aa4-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="63aa4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="63aa4-112">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="63aa4-112">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="63aa4-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="63aa4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="63aa4-114">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="63aa4-114">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="63aa4-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="63aa4-115">Application</span></span> | <span data-ttu-id="63aa4-116">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="63aa4-116">MailboxSettings.ReadWrite</span></span> |


## <a name="http-request"></a><span data-ttu-id="63aa4-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="63aa4-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/mailFolders/inbox/messageRules
POST /users/{id | userPrincipalName}/mailFolders/inbox/messageRules
```
## <a name="request-headers"></a><span data-ttu-id="63aa4-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="63aa4-118">Request headers</span></span>
| <span data-ttu-id="63aa4-119">Nome</span><span class="sxs-lookup"><span data-stu-id="63aa4-119">Name</span></span>       | <span data-ttu-id="63aa4-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="63aa4-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="63aa4-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="63aa4-121">Authorization</span></span>  | <span data-ttu-id="63aa4-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="63aa4-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="63aa4-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="63aa4-124">Request body</span></span>
<span data-ttu-id="63aa4-125">No corpo da solicitação, forneça os parâmetros que são aplicáveis à sua regra.</span><span class="sxs-lookup"><span data-stu-id="63aa4-125">In the request body, supply the parameters that are applicable to your rule.</span></span> <span data-ttu-id="63aa4-126">A seguir estão os parâmetros de corpo que normalmente são usados ao criar regras.</span><span class="sxs-lookup"><span data-stu-id="63aa4-126">The following are body parameters that are typically used when creating rules.</span></span> <span data-ttu-id="63aa4-127">É possível especificar outras propriedades **messageRule** graváveis conforme apropriado no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="63aa4-127">You can specify any other writable **messageRule** properties as appropriate in the request body.</span></span>

| <span data-ttu-id="63aa4-128">Nome</span><span class="sxs-lookup"><span data-stu-id="63aa4-128">Name</span></span>       | <span data-ttu-id="63aa4-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="63aa4-129">Type</span></span>|<span data-ttu-id="63aa4-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="63aa4-130">Description</span></span>|
|:--------|:-------|:----------|
|<span data-ttu-id="63aa4-131">actions</span><span class="sxs-lookup"><span data-stu-id="63aa4-131">actions</span></span>|[<span data-ttu-id="63aa4-132">messageRuleActions</span><span class="sxs-lookup"><span data-stu-id="63aa4-132">messageRuleActions</span></span>](../resources/messageruleactions.md)|<span data-ttu-id="63aa4-133">Ações a serem realizadas em uma mensagem quando as condições correspondentes, se houver, forem atendidas.</span><span class="sxs-lookup"><span data-stu-id="63aa4-133">Actions to be taken on a message when the corresponding conditions, if any, are fulfilled.</span></span> <span data-ttu-id="63aa4-134">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="63aa4-134">Required.</span></span>|
|<span data-ttu-id="63aa4-135">conditions</span><span class="sxs-lookup"><span data-stu-id="63aa4-135">conditions</span></span>|[<span data-ttu-id="63aa4-136">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="63aa4-136">messageRulePredicates</span></span>](../resources/messagerulepredicates.md)|<span data-ttu-id="63aa4-137">Condições que, quando atendidas, acionarão as ações correspondentes dessa regra.</span><span class="sxs-lookup"><span data-stu-id="63aa4-137">Conditions that when fulfilled, will trigger the corresponding actions for that rule.</span></span> <span data-ttu-id="63aa4-138">Opcional.</span><span class="sxs-lookup"><span data-stu-id="63aa4-138">Optional.</span></span>|
|<span data-ttu-id="63aa4-139">displayName</span><span class="sxs-lookup"><span data-stu-id="63aa4-139">displayName</span></span>| <span data-ttu-id="63aa4-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="63aa4-140">String</span></span>  | <span data-ttu-id="63aa4-141">O nome de exibição da regra.</span><span class="sxs-lookup"><span data-stu-id="63aa4-141">The display name of the rule.</span></span> <span data-ttu-id="63aa4-142">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="63aa4-142">Required.</span></span>|
|<span data-ttu-id="63aa4-143">exceptions</span><span class="sxs-lookup"><span data-stu-id="63aa4-143">exceptions</span></span>| [<span data-ttu-id="63aa4-144">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="63aa4-144">messageRulePredicates</span></span>](../resources/messagerulepredicates.md)| <span data-ttu-id="63aa4-145">Representa condições de exceção para a regra.</span><span class="sxs-lookup"><span data-stu-id="63aa4-145">Represents exception conditions for the rule.</span></span> <span data-ttu-id="63aa4-146">Opcional.</span><span class="sxs-lookup"><span data-stu-id="63aa4-146">Optional.</span></span> |
|<span data-ttu-id="63aa4-147">isEnabled</span><span class="sxs-lookup"><span data-stu-id="63aa4-147">isEnabled</span></span> | <span data-ttu-id="63aa4-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="63aa4-148">Boolean</span></span> | <span data-ttu-id="63aa4-149">Indica se a regra está habilitada para ser aplicada a mensagens.</span><span class="sxs-lookup"><span data-stu-id="63aa4-149">Indicates whether the rule is enabled to be applied to messages.</span></span> <span data-ttu-id="63aa4-150">Opcional.</span><span class="sxs-lookup"><span data-stu-id="63aa4-150">Optional.</span></span> |
|<span data-ttu-id="63aa4-151">sequence</span><span class="sxs-lookup"><span data-stu-id="63aa4-151">sequence</span></span>| <span data-ttu-id="63aa4-152">Int32</span><span class="sxs-lookup"><span data-stu-id="63aa4-152">Int32</span></span> | <span data-ttu-id="63aa4-153">Indica a ordem em que a regra é executada, entre outras regras.</span><span class="sxs-lookup"><span data-stu-id="63aa4-153">Indicates the order in which the rule is executed, among other rules.</span></span> <span data-ttu-id="63aa4-154">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="63aa4-154">Required.</span></span>|

## <a name="response"></a><span data-ttu-id="63aa4-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="63aa4-155">Response</span></span>
<span data-ttu-id="63aa4-156">Se bem-sucedido, esse método retornará um código de resposta `201 Created` e um objeto **messageRule** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="63aa4-156">If successful, this method returns `201 Created` response code and a **messageRule** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="63aa4-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="63aa4-157">Example</span></span>
##### <a name="request"></a><span data-ttu-id="63aa4-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="63aa4-158">Request</span></span>
<span data-ttu-id="63aa4-159">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="63aa4-159">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="63aa4-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="63aa4-160">Response</span></span>
<span data-ttu-id="63aa4-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="63aa4-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->