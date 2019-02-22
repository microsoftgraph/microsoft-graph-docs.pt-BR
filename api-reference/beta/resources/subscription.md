---
title: tipo de recurso Subscription
description: 'Uma assinatura permite que um aplicativo cliente receba notificações sobre alterações nos dados no Microsoft Graph. No momento, as assinaturas estão habilitadas para os seguintes recursos:'
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 9de48cc6a3e5dde459673117d9ee00a34477faf6
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30163935"
---
# <a name="subscription-resource-type"></a>tipo de recurso Subscription

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma assinatura permite que um aplicativo cliente receba notificações sobre alterações nos dados no Microsoft Graph. No momento, as assinaturas estão habilitadas para os seguintes recursos:

- Uma [mensagem][], [evento][]ou [contato][] no Outlook
- Uma [conversa][] de um grupo do Office 365
- Conteúdo na hierarquia de uma pasta raiz [driveItem][] no onedrive for Business ou em uma pasta raiz ou subpasta [driveItem][] no onedrive pessoal de um usuário
- Um [usuário][] ou [grupo][] no Azure Active Directory
- Um [alerta][] da API de segurança do Microsoft Graph


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.subscription"
}-->

```json
{
  "changeType": "string",
  "notificationUrl": "string",
  "resource": "string",
  "applicationId" : "string",
  "expirationDateTime": "string (timestamp)",
  "id": "string (identifier)",
  "clientState": "string",
  "creatorId": "string"
}
```

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------|:-----|:------------|
| changeType | string | Obrigatório. Indica o tipo de alteração no recurso inscrito que gerará uma notificação. Os valores com suporte são: `created`, `updated`, `deleted`. Vários valores podem ser combinados usando uma lista separada por vírgula. <br><br>Observação: as notificações de item raiz da unidade `updated` dão suporte somente a ChangeType. Suporte e `deleted` ChangeType para `updated` notificações de grupo e usuário. |
| notificationUrl | cadeia de caracteres | Obrigatório. A URL do ponto de extremidade que receberá as notificações. Essa URL deve fazer uso do protocolo HTTPS. |
| recurso | string | Obrigatório. Especifica o recurso que será monitorado para alterações. Não inclua a URL base (`https://graph.microsoft.com/beta/`). |
| expirationDateTime | DateTimeOffset | Obrigatório. Especifica a data e a hora em que a assinatura de webhook expira. O horário está em UTC e pode ser uma quantidade de tempo desde a criação da assinatura que varia para o recurso assinado.  Confira na tabela abaixo o tempo máximo permitido para a assinatura. |
| clientState | string | Opcional. Especifica o valor da propriedade `clientState` enviada pelo serviço em cada notificação. O tamanho máximo é de 255 caracteres. O cliente pode verificar se a notificação foi proveniente do serviço comparando o valor da propriedade `clientState` enviada com a assinatura com o valor da propriedade `clientState` recebida com cada notificação. |
| id | string | Identificador exclusivo da assinatura. Somente leitura. |
| ApplicationId | string | Identificador do aplicativo usado para criar a assinatura. Somente leitura. |
| creatorId | string | Identificador da entidade de serviço ou usuário que criou a assinatura. Se o aplicativo usou permissões delegadas para criar a assinatura, este campo conterá a ID do usuário conectado o aplicativo chamado em nome de. Se o aplicativo usava permissões de aplicativo, este campo contém a ID da entidade de serviço correspondente ao aplicativo. Somente leitura. |

## <a name="maximum-length-of-subscription-per-resource-type"></a>Tamanho máximo da assinatura por tipo de recurso

| Recurso            | Tempo de Expiração Máximo  |
|:--------------------|:-------------------------|
| Email                | 4230 minutos (abaixo de 3 dias)    |
| Calendário            | 4230 minutos (abaixo de 3 dias)    |
| Contatos            | 4230 minutos (abaixo de 3 dias)    |
| Conversas em grupo | 4230 minutos (abaixo de 3 dias)    |
| Itens raiz de unidade    | 4230 minutos (abaixo de 3 dias)    |
| Alertas de segurança     | 43200 minutos (menos de 30 dias)  |

> **Observação:** Aplicativos existentes e novos aplicativos não devem exceder o valor com suporte. No futuro, todas as solicitações para criar ou renovar uma assinatura além do valor máximo falharão.

## <a name="relationships"></a>Relações

Nenhum

## <a name="methods"></a>Métodos

| Método | Tipo de retorno | Descrição |
|:-------|:------------|:------------|
| [Criar assinatura](../api/subscription-post-subscriptions.md) | [subscription](subscription.md) | Assina um aplicativo de escuta para receber notificações quando dados do Microsoft Graph são alterados. |
| [Atualizar assinatura](../api/subscription-update.md) | [subscription](subscription.md) | ReNovar uma assinatura atualizando seu tempo de expiração. |
| [Listar assinaturas](../api/subscription-list.md) | [subscription](subscription.md) | Lista assinaturas ativas. |
| [Obter assinatura](../api/subscription-get.md) | [subscription](subscription.md) | Leia as propriedades e as relações do objeto Subscription. |
| [Excluir assinatura](../api/subscription-delete.md) | Nenhuma | Excluir um objeto Subscription. |

[contato]: ./contact.md
[conversa]: ./conversation.md
[driveItem]: ./driveitem.md
[event]: ./event.md
[group]: ./group.md
[message]: ./message.md
[user]: ./user.md
[alert]: ./alert.md

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "subscription resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/subscription.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
