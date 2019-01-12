---
title: tipo de recurso de assinatura
description: 'Uma assinatura permite que um aplicativo cliente receber notificações sobre as alterações de dados no Microsoft Graph. Atualmente, as assinaturas são habilitadas para os seguintes recursos:'
localization_priority: Priority
author: piotrci
ms.openlocfilehash: 7837524f2ce20a24154b84a82537ec6a4149bfe9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917815"
---
# <a name="subscription-resource-type"></a>tipo de recurso de assinatura

Uma assinatura permite que um aplicativo cliente receber notificações sobre as alterações de dados no Microsoft Graph. Atualmente, as assinaturas são habilitadas para os seguintes recursos:

- Email, eventos e contatos do Outlook.
- Conversas de Grupos do Office.
- Itens raiz da unidade do OneDrive.
- Usuários e grupos do Azure Active Directory.
- Alertas do API de segurança do Microsoft Graph.

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.subscription",
  "@odata.annotations": [
    {
      "capabilities": {
        "skippable": false,
        "toppable": false,
        "countable": false,
        "expandable": false,
        "filterable": false,
        "referenceable": false,
        "selectable": false,
        "sortable": false
      }
    }
  ]
}-->

```json
{
  "changeType": "string",
  "notificationUrl": "string",
  "resource": "string",
  "applicationId" : "string",
  "expirationDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "clientState": "string",
  "creatorId": "string"
}
```

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------|:-----|:------------|
| changeType | string | Obrigatório. Indica o tipo de alteração no recurso inscrito que gerará uma notificação. Os valores com suporte são: `created`, `updated`, `deleted`. Vários valores podem ser combinados usando uma lista separada por vírgula.<br><br>Observação: Notificações de item de raiz de unidade suportam somente a `updated` changeType. Suportam a notificações de usuário e grupo `updated` e `deleted` changeType.|
| notificationUrl | string | Obrigatório. A URL do ponto de extremidade que receberá as notificações. Essa URL deve tornar a usar o HTTPS protocolo. |
| recurso | string | Obrigatório. Especifica o recurso que será monitorado para que as alterações. Não incluir a URL base (`https://graph.microsoft.com/v1.0/`). |
| expirationDateTime | [dateTime](https://tools.ietf.org/html/rfc3339) | Obrigatório. Especifica a data e a hora em que a assinatura de webhook expira. O horário está em UTC e pode ser uma quantidade de tempo desde a criação da assinatura que varia para o recurso assinado.  Confira na tabela abaixo o tempo máximo permitido para a assinatura. |
| clientState | string | Opcional. Especifica o valor da propriedade `clientState` enviada pelo serviço em cada notificação. O comprimento máximo é de 128 caracteres. O cliente pode verificar se a notificação foi proveniente do serviço comparando o valor da propriedade `clientState` enviada com a assinatura com o valor da propriedade `clientState` recebida com cada notificação. |
| id | string | Identificador exclusivo da assinatura. Somente leitura. |
| ApplicationId | string | Identificador do aplicativo usado para criar a inscrição. Somente leitura. |
| creatorId | string | Identificador do usuário ou da entidade de serviço que criou a assinatura. Se o aplicativo usado delegadas permissões para criar a assinatura, esse campo contém a id do usuário entrou no de que aplicativo chamado em nome. Se o aplicativo usado permissões de aplicativo, esse campo contém a id da entidade de serviço correspondente para o aplicativo. Somente leitura. |

## <a name="maximum-length-of-subscription-per-resource-type"></a>Tamanho máximo da assinatura por tipo de recurso

| Recurso            | Tempo de Expiração Máximo  |
|:--------------------|:-------------------------|
| Email                | 4230 minutos (em 3 dias)    |
| Calendário            | 4230 minutos (em 3 dias)    |
| Contatos            | 4230 minutos (em 3 dias)    |
| Conversas em grupo | 4230 minutos (em 3 dias)    |
| Itens raiz de unidade    | 4230 minutos (em 3 dias)    |
| Alertas de segurança     | 43200 minutos (em 30 dias)  |

> **Observação:** Aplicativos existentes e novos não deve exceder o valor com suporte. No futuro, quaisquer solicitações para criar ou renovar uma assinatura além o valor máximo falhará.

## <a name="relationships"></a>Relações

Nenhum

## <a name="methods"></a>Métodos

| Método | Tipo de retorno | Descrição |
|:-------|:------------|:------------|
| [Criar assinatura](../api/subscription-post-subscriptions.md) | [subscription](subscription.md) | Assina um aplicativo de escuta para receber notificações quando dados do Microsoft Graph são alterados. |
| [Atualizar assinatura](../api/subscription-update.md) | [subscription](subscription.md) | Renova uma assinatura atualizando seu tempo de expiração. |
| [Inscrições de lista](../api/subscription-list.md) | [subscription](subscription.md) | Lista inscrições ativas. |
| [Obter assinatura](../api/subscription-get.md) | [subscription](subscription.md) | Lê as propriedades e as relações do objeto subscription. |
| [Excluir assinatura](../api/subscription-delete.md) | Nenhuma |Exclui um objeto subscription. |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "subscription resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
