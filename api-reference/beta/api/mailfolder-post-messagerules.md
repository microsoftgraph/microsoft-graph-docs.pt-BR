---
title: Criar regra
description: 'Crie um objeto messageRule especificando um conjunto de condições e ações. '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 7d59d8c5a173f614473a7443fc7db97a4e3f6618
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36415225"
---
# <a name="create-rule"></a>Criar regra

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Crie um objeto [messageRule](../resources/messagerule.md) especificando um conjunto de condições e ações. 

O Outlook realizará essas ações se uma mensagem recebida na Caixa de Entrada do usuário atender às condições especificadas.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | MailboxSettings.ReadWrite    |
|Delegado (conta pessoal da Microsoft) | MailboxSettings.ReadWrite    |
|Aplicativo | MailboxSettings.ReadWrite |


## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /me/mailFolders/inbox/messagerules
POST /users/{id | userPrincipalName}/mailFolders/inbox/messagerules
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome       | Descrição|
|:---------------|:----------|
| Autorização  | {token} de portador. Obrigatório. |


## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça os parâmetros que são aplicáveis à sua regra. A seguir estão os parâmetros de corpo que normalmente são usados ao criar regras. É possível especificar outras propriedades **messageRule** graváveis conforme apropriado no corpo da solicitação.

| Parâmetro       | Tipo|Descrição|
|:--------|:-------|:----------|
|actions|[messageRuleActions](../resources/messageruleactions.md)|Ações a serem realizadas em uma mensagem quando as condições correspondentes, se houver, forem atendidas. Obrigatório.|
|conditions|[messageRulePredicates](../resources/messagerulepredicates.md)|Condições que, quando atendidas, acionarão as ações correspondentes dessa regra. Opcional.|
|displayName| String  | O nome de exibição da regra. Obrigatório.|
|exceptions| [messageRulePredicates](../resources/messagerulepredicates.md)| Representa condições de exceção para a regra. Opcional. |
|isEnabled | Boolean | Indica se a regra está habilitada para ser aplicada a mensagens. Opcional. |
|sequence| Int32 | Indica a ordem em que a regra é executada, entre outras regras. Obrigatório.|

## <a name="response"></a>Resposta
Se bem-sucedido, esse método retornará um código de resposta `201 Created` e um objeto **messageRule** no corpo da resposta.

## <a name="example"></a>Exemplo
##### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.

# <a name="httptabhttp"></a>[HTTP](#tab/http)
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
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-messagerule-from-mailfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-messagerule-from-mailfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[Objetivo-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-messagerule-from-mailfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
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
