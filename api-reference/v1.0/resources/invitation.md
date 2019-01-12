---
title: gerenciador de convites
description: 'Use o gerenciador de convites para criar um convite para adicionar um usuário externo à organização. '
localization_priority: Priority
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0a0ee3ba23cb0c323a660b9afd26fa044a50897c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27976734"
---
# <a name="invitation-manager"></a>gerenciador de convites

Use o gerenciador de convites para criar um convite para adicionar um usuário externo à organização. 

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
|invitedUserEmailAddress|String|O endereço de email do usuário que está sendo convidado. Obrigatório.|
|invitedUserMessageInfo|[invitedUserMessageInfo](invitedusermessageinfo.md)|Configurações adicionais para a mensagem que está sendo enviada ao usuário convidado, incluindo a lista de destinatários cc, o idioma e o texto da mensagem de personalização.|
|sendInvitationMessage|Booliano|Indica se um email deve ser enviado ao usuário que está sendo convidado ou não. O padrão é false.|
|inviteRedirectUrl|String|A URL para a qual o usuário deve ser redirecionado após o resgate do convite. Obrigatório.|
|inviteRedeemUrl|String|A URL que o usuário pode usar para resgatar o convite. Somente leitura|
|invitedUserType|String|O userType do usuário que está sendo convidado. Por padrão, é Convidado. Você poderá convidar como Membro se não for administrador da empresa. |
|status|String|O status do convite. Valores possíveis: PendingAcceptance, Completed, InProgress, e Error|

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
