---
title: tipo de recurso de assinatura
description: 'Uma assinatura permite que um aplicativo cliente receba notificações sobre dados no Microsoft Graph. Atualmente, as assinaturas estão habilitadas para as seguintes coleções de recursos:'
localization_priority: Priority
author: piotrci
ms.openlocfilehash: db3a536395f327115af69f769f37c823013ec7fa
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563697"
---
# <a name="subscription-resource-type"></a>tipo de recurso de assinatura

Uma assinatura permite que um aplicativo cliente receba notificações sobre dados no Microsoft Graph. Atualmente, as assinaturas estão habilitadas para as seguintes coleções de recursos:

- Um [mensagem][], [evento][], ou [contato][] no Outlook
- Um [conversa][] de um grupo do Office 365
- Conteúdo da hierarquia de uma pasta raiz [driveItem][] no OneDrive for Business ou de uma pasta raiz ou uma subpasta [driveItem][] no OneDrive pessoal do usuário
- Um [usuário][] ou [grupo][] no Azure Active Directory
- Um [alerta][] da API de Segurança do Microsoft Graph

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
| changeType | cadeia de caracteres | Obrigatório. Indica o tipo de alteração no recurso inscrito que gerará uma notificação. Os valores com suporte são: `created`, `updated`, `deleted`. Vários valores podem ser combinados usando uma lista separada por vírgula.<br><br>Observação: As notificações do item na raiz da unidade suportam somente `updated` changeType. Notificações de grupos e usuário suportam `updated` e `deleted` changeType.|
| notificationUrl | cadeia de caracteres | Obrigatório. A URL do ponto de extremidade que receberá as notificações. Esta URL deve usar o protocolo HTTPS. |
| recurso | cadeia de caracteres | Obrigatório. Especifica o recurso que será monitorado para detectar alterações. Não incluir a URL base (`https://graph.microsoft.com/v1.0/`). |
| expirationDateTime | [dateTime](https://tools.ietf.org/html/rfc3339) | Obrigatório. Especifica a data e a hora em que a assinatura do webhook expira. O horário está em UTC e pode ser uma quantidade de tempo desde a criação da assinatura que varia para o recurso assinado.  Confira na tabela abaixo o tempo máximo permitido para a assinatura. |
| clientState | string | Opcional. Especifica o valor da propriedade `clientState` enviada pelo serviço em cada notificação. O comprimento máximo é de 128 caracteres. O cliente pode verificar se a notificação foi proveniente do serviço comparando o valor da propriedade `clientState` enviada com a assinatura com o valor da propriedade `clientState` recebida com cada notificação. |
| id | string | Identificador exclusivo da assinatura. Somente leitura. |
| ApplicationId | cadeia de caracteres | Identificador do aplicativo usado para criar a assinatura. Somente leitura. |
| creatorId | cadeia de caracteres | Identificador de usuário ou entidade de serviço que criou a assinatura. Se o aplicativo usado delegada permissões para criar a assinatura, esse campo contém a id do usuário que entrou no aplicativo chamado em nome dele. Se o aplicativo usou permissões do aplicativo, esse campo contém a id da entidade de serviço correspondente ao aplicativo. Somente leitura. |

## <a name="maximum-length-of-subscription-per-resource-type"></a>Tamanho máximo da assinatura por tipo de recurso

| Recurso            | Tempo de Expiração Máximo  |
|:--------------------|:-------------------------|
| Email                | 4230 minutos (em 3 dias)    |
| Calendário            | 4230 minutos (em 3 dias)    |
| Contatos            | 4230 minutos (em 3 dias)    |
| Conversas em grupo | 4230 minutos (em 3 dias)    |
| Itens raiz de unidade    | 4230 minutos (em 3 dias)    |
| Alertas de segurança     | 43200 minutos (em 30 dias )  |

> **Observação:** Os aplicativos existentes e os novos aplicativos não devem ultrapassar o valor suportado. No futuro, as solicitações para criar ou renovar uma assinatura além do valor máximo falharão.

## <a name="relationships"></a>Relações

Nenhuma

## <a name="methods"></a>Métodos

| Método | Tipo de retorno | Descrição |
|:-------|:------------|:------------|
| [Criar assinatura](../api/subscription-post-subscriptions.md) | [subscription](subscription.md) | Assina um aplicativo de escuta para receber notificações quando dados do Microsoft Graph são alterados. |
| [Atualizar assinatura](../api/subscription-update.md) | [subscription](subscription.md) | Renova uma assinatura atualizando seu tempo de expiração. |
| [Listar de assinaturas](../api/subscription-list.md) | [assinatura](subscription.md) | Lista assinaturas ativas. |
| [Obter assinatura](../api/subscription-get.md) | [subscription](subscription.md) | Lê as propriedades e as relações do objeto subscription. |
| [Excluir assinatura](../api/subscription-delete.md) | Nenhuma |Exclui um objeto assinatura. |

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
<!-- {
  "type": "#page.annotation",
  "description": "subscription resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
