---
title: tipo de recurso convite
description: Representa um convite usado para adicionar usuários externos a uma organização.
localization_priority: Priority
author: Sammak
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: ff977732b4d0894767f06ccfcf03451a8cc77f61
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50941362"
---
# <a name="invitation-resource-type"></a>tipo de recurso convite

Namespace: microsoft.graph

Representa um convite usado para adicionar usuários externos a uma organização. 

O processo de convite usa o fluxo a seguir:

* Um convite é criado
* Um convite é enviado ao usuário convidado (contendo um link do convite)
* O usuário convidado clica no link do convite, entra e recupera o convite, e a criação da entidade de usuário que representa o usuário convidado é concluída
* O usuário é redirecionado para uma página específica após a conclusão do resgate

A criação de um convite retornará uma URL de resgate na resposta (*inviteRedeemUrl*). A API de criação de convite pode enviar automaticamente um email que contém a URL de resgate ao usuário convidado, definindo-se *sendInvitationMessage* como true. Você também pode personalizar a mensagem será enviada ao usuário convidado. Em vez disso, se você desejar enviar a URL de resgate por outros meios, poderá definir *sendInvitationMessage* como false e usar a URL de resgate da resposta para criar sua própria comunicação. Atualmente, não há qualquer API para execução do processo de resgate. O usuário convidado tem que clicar no link *inviteRedeemUrl* enviado na comunicação na etapa anterior e passar pelo processo de resgate interativo em um navegador. Após a conclusão, o usuário convidado torna-se um usuário externo na organização.


## <a name="methods"></a>Métodos
| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Criar convite](../api/invitation-post.md) | invitation | Escreva as propriedades e os relacionamentos do objeto invitation.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|invitedUserDisplayName|String|O nome de exibição do usuário que está sendo convidado.|
|invitedUserEmailAddress|String|O endereço de email do usuário que está sendo convidado. Obrigatório. Os seguintes caracteres especiais não são permitidos no endereço de email:<br><ul><li>Til (~)</li><li>Ponto de exclamação (`!`)</li><li>Hashtag (`#`)</li><li>Cifrão (`$`)</li><li>Percentagem (`%`)</li><li>Acento circunflexo (`^`)</li><li>E comercial (`&`)</li><li>Asterisco (`*`)</li><li>Parênteses (`( )`)</li><li>Sinal de mais (`+`)</li><li>Sinal de igualdade (`=`)</li><li>Colchetes (`[ ]`)</li><li>Chaves (`{ }`)</li><li>Barra invertida (`\`)</li><li>Barra (`/`)</li><li>Barra vertical (`\|`)</li><li>Ponto e vírgula (`;`)</li><li>Dois pontos (`:`)</li><li>Aspas (`"`)</li><li>Sinais de maior-que e menor-que(`< >`)</li><li>Sinal de interrogação (`?`)</li><li>Vírgula (`,`)</li></ul><br>No entanto, as seguintes exceções se aplicam:<br><ul><li>Um ponto (`.`) ou um hífen (`-`) é permitido em qualquer lugar no nome de usuário, exceto no início ou no final do nome.</li><li>Um underline (`_`) é permitido em qualquer lugar no nome de usuário. Isso inclui no início ou no final do nome.</li></ul>|
|invitedUserMessageInfo|[invitedUserMessageInfo](invitedusermessageinfo.md)|Configurações adicionais para a mensagem que está sendo enviada ao usuário convidado, incluindo a lista de destinatários cc, o idioma e o texto da mensagem de personalização.|
|sendInvitationMessage|Boolean|Indica se um email deve ser enviado ao usuário que está sendo convidado ou não. O padrão é false.|
|inviteRedirectUrl|Cadeia de caracteres|O URL para a qual o usuário deve ser redirecionado uma vez que o convite seja resgatado. Obrigatório.|
|inviteRedeemUrl|Cadeia de caracteres|O URL que o usuário pode usar para resgatar seus convites. Somente leitura|.
|invitedUserType|String|O userType do usuário que está sendo convidado. Por padrão, é `Guest` Você pode convidar como `Member` se fosse um administrador da empresa. |
|status|Cadeia de caracteres|O status do convite. Os valores possíveis são: `PendingAcceptance`, `Completed`, `InProgress` e `Error`|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|invitedUser|[User](user.md)|O usuário criado como parte da criação do convite. Somente leitura|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso

<!-- { "blockType": "resource", "baseType": "microsoft.graph.entity", "@odata.type": "microsoft.graph.invitation" } -->
```json
{
  "invitedUserDisplayName": "string",
  "invitedUserEmailAddress": "string",
  "invitedUserMessageInfo": {"@odata.type": "microsoft.graph.invitedUserMessageInfo"},
  "sendInvitationMessage": false,
  "inviteRedirectUrl": "string",
  "inviteRedeemUrl": "string",
  "status": "string",
  "invitedUser": {"@odata.type": "microsoft.graph.user"},
  "invitedUserType": "string"
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2016-22-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "invitation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

