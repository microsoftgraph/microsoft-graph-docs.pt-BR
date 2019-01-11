---
title: Criar regra
description: 'Crie um objeto messageRule especificando um conjunto de condições e ações. '
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 34224240ec931bdc07e3ad8a262528f94600393b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27821046"
---
# <a name="create-rule"></a><span data-ttu-id="aa764-103">Criar regra</span><span class="sxs-lookup"><span data-stu-id="aa764-103">Create rule</span></span>

> <span data-ttu-id="aa764-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="aa764-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="aa764-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="aa764-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="aa764-106">Crie um objeto [messageRule](../resources/messagerule.md) especificando um conjunto de condições e ações.</span><span class="sxs-lookup"><span data-stu-id="aa764-106">Create a [messageRule](../resources/messagerule.md) object by specifying a set of conditions and actions.</span></span> 

<span data-ttu-id="aa764-107">O Outlook realizará essas ações se uma mensagem recebida na Caixa de Entrada do usuário atender às condições especificadas.</span><span class="sxs-lookup"><span data-stu-id="aa764-107">Outlook carries out those actions if an incoming message in the user's Inbox meets the specified conditions.</span></span>

## <a name="permissions"></a><span data-ttu-id="aa764-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="aa764-108">Permissions</span></span>
<span data-ttu-id="aa764-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aa764-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aa764-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="aa764-111">Permission type</span></span>      | <span data-ttu-id="aa764-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="aa764-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aa764-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="aa764-113">Delegated (work or school account)</span></span> | <span data-ttu-id="aa764-114">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aa764-114">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="aa764-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="aa764-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aa764-116">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aa764-116">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="aa764-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="aa764-117">Application</span></span> | <span data-ttu-id="aa764-118">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aa764-118">MailboxSettings.ReadWrite</span></span> |


## <a name="http-request"></a><span data-ttu-id="aa764-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="aa764-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/mailFolders/inbox/messagerules
POST /users/{id | userPrincipalName}/mailFolders/inbox/messagerules
```
## <a name="request-headers"></a><span data-ttu-id="aa764-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="aa764-120">Request headers</span></span>
| <span data-ttu-id="aa764-121">Nome</span><span class="sxs-lookup"><span data-stu-id="aa764-121">Name</span></span>       | <span data-ttu-id="aa764-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="aa764-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="aa764-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="aa764-123">Authorization</span></span>  | <span data-ttu-id="aa764-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="aa764-p103">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="aa764-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="aa764-126">Request body</span></span>
<span data-ttu-id="aa764-127">No corpo da solicitação, forneça os parâmetros que são aplicáveis à sua regra.</span><span class="sxs-lookup"><span data-stu-id="aa764-127">In the request body, supply the parameters that are applicable to your rule.</span></span> <span data-ttu-id="aa764-128">A seguir estão os parâmetros de corpo que normalmente são usados ao criar regras.</span><span class="sxs-lookup"><span data-stu-id="aa764-128">The following are body parameters that are typically used when creating rules.</span></span> <span data-ttu-id="aa764-129">É possível especificar outras propriedades **messageRule** graváveis conforme apropriado no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="aa764-129">You can specify any other writable **messageRule** properties as appropriate in the request body.</span></span>

| <span data-ttu-id="aa764-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="aa764-130">Parameter</span></span>       | <span data-ttu-id="aa764-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="aa764-131">Type</span></span>|<span data-ttu-id="aa764-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="aa764-132">Description</span></span>|
|:--------|:-------|:----------|
|<span data-ttu-id="aa764-133">actions</span><span class="sxs-lookup"><span data-stu-id="aa764-133">actions</span></span>|[<span data-ttu-id="aa764-134">messageRuleActions</span><span class="sxs-lookup"><span data-stu-id="aa764-134">messageRuleActions</span></span>](../resources/messageruleactions.md)|<span data-ttu-id="aa764-135">Ações a serem realizadas em uma mensagem quando as condições correspondentes, se houver, forem atendidas.</span><span class="sxs-lookup"><span data-stu-id="aa764-135">Actions to be taken on a message when the corresponding conditions, if any, are fulfilled.</span></span> <span data-ttu-id="aa764-136">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="aa764-136">Required.</span></span>|
|<span data-ttu-id="aa764-137">conditions</span><span class="sxs-lookup"><span data-stu-id="aa764-137">conditions</span></span>|[<span data-ttu-id="aa764-138">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="aa764-138">messageRulePredicates</span></span>](../resources/messagerulepredicates.md)|<span data-ttu-id="aa764-139">Condições que, quando atendidas, acionarão as ações correspondentes dessa regra.</span><span class="sxs-lookup"><span data-stu-id="aa764-139">Conditions that when fulfilled, will trigger the corresponding actions for that rule.</span></span> <span data-ttu-id="aa764-140">Opcional.</span><span class="sxs-lookup"><span data-stu-id="aa764-140">Optional.</span></span>|
|<span data-ttu-id="aa764-141">displayName</span><span class="sxs-lookup"><span data-stu-id="aa764-141">displayName</span></span>| <span data-ttu-id="aa764-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="aa764-142">String</span></span>  | <span data-ttu-id="aa764-143">O nome de exibição da regra.</span><span class="sxs-lookup"><span data-stu-id="aa764-143">The display name of the rule.</span></span> <span data-ttu-id="aa764-144">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="aa764-144">Required.</span></span>|
|<span data-ttu-id="aa764-145">exceptions</span><span class="sxs-lookup"><span data-stu-id="aa764-145">exceptions</span></span>| [<span data-ttu-id="aa764-146">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="aa764-146">messageRulePredicates</span></span>](../resources/messagerulepredicates.md)| <span data-ttu-id="aa764-147">Representa condições de exceção para a regra.</span><span class="sxs-lookup"><span data-stu-id="aa764-147">Represents exception conditions for the rule.</span></span> <span data-ttu-id="aa764-148">Opcional.</span><span class="sxs-lookup"><span data-stu-id="aa764-148">Optional.</span></span> |
|<span data-ttu-id="aa764-149">isEnabled</span><span class="sxs-lookup"><span data-stu-id="aa764-149">isEnabled</span></span> | <span data-ttu-id="aa764-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="aa764-150">Boolean</span></span> | <span data-ttu-id="aa764-151">Indica se a regra está habilitada para ser aplicada a mensagens.</span><span class="sxs-lookup"><span data-stu-id="aa764-151">Indicates whether the rule is enabled to be applied to messages.</span></span> <span data-ttu-id="aa764-152">Opcional.</span><span class="sxs-lookup"><span data-stu-id="aa764-152">Optional.</span></span> |
|<span data-ttu-id="aa764-153">sequence</span><span class="sxs-lookup"><span data-stu-id="aa764-153">sequence</span></span>| <span data-ttu-id="aa764-154">Int32</span><span class="sxs-lookup"><span data-stu-id="aa764-154">Int32</span></span> | <span data-ttu-id="aa764-155">Indica a ordem em que a regra é executada, entre outras regras.</span><span class="sxs-lookup"><span data-stu-id="aa764-155">Indicates the order in which the rule is executed, among other rules.</span></span> <span data-ttu-id="aa764-156">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="aa764-156">Required.</span></span>|

## <a name="response"></a><span data-ttu-id="aa764-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="aa764-157">Response</span></span>
<span data-ttu-id="aa764-158">Se bem-sucedido, esse método retornará um código de resposta `201 Created` e um objeto **messageRule** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="aa764-158">If successful, this method returns `201 Created` response code and a **messageRule** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aa764-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="aa764-159">Example</span></span>
##### <a name="request"></a><span data-ttu-id="aa764-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aa764-160">Request</span></span>
<span data-ttu-id="aa764-161">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="aa764-161">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="aa764-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="aa764-162">Response</span></span>
<span data-ttu-id="aa764-p111">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="aa764-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
