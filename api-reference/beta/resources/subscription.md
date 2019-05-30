---
title: tipo de recurso de assinatura
description: 'Uma assinatura permite que um aplicativo cliente receba notificações sobre dados no Microsoft Graph. Atualmente, as assinaturas estão habilitadas para as seguintes coleções de recursos:'
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 6a7fd50a53e68313ba72c8bd5d90b47d2b5b2607
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/29/2019
ms.locfileid: "34537202"
---
# <a name="subscription-resource-type"></a>tipo de recurso de assinatura

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma assinatura permite que um aplicativo cliente receba notificações sobre dados no Microsoft Graph. Atualmente, as assinaturas estão habilitadas para as seguintes coleções de recursos:

- Um [mensagem][], [evento][], ou [contato][] no Outlook
- Um [conversa][] de um grupo do Office 365
- Conteúdo da hierarquia de uma pasta raiz [driveItem][] no OneDrive for Business ou de uma pasta raiz ou uma subpasta [driveItem][] no OneDrive pessoal do usuário
- Um [usuário][] ou [grupo][] no Azure Active Directory
- Um [alerta][] da API de Segurança do Microsoft Graph


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
  "lifecycleNotificationUrl": "string",
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
| changeType | cadeia de caracteres | Obrigatório. Indica o tipo de alteração no recurso inscrito que gerará uma notificação. Os valores com suporte são: `created`, `updated`, `deleted`. Vários valores podem ser combinados usando uma lista separada por vírgula. <br><br>Observação: As notificações do item na raiz da unidade suportam somente `updated` changeType. Notificações de grupos e usuário suportam `updated` e `deleted` changeType. |
| notificationUrl | cadeia de caracteres | Obrigatório. A URL do ponto de extremidade que recebe as notificações. Esta URL deve usar o protocolo HTTPS. |
| lifecycleNotificationUrl | cadeia de caracteres | Opcional. A URL do ponto de extremidade que recebe notificações de ciclo `subscriptionRemoved` de `missed` vida, incluindo e notificações. Se não for fornecido, as notificações serão entregues ao **notificationUrl**. [Leia mais](/graph/webhooks-outlook-authz.md) sobre como os recursos do Outlook usam notificações de ciclo de vida.  Esta URL deve usar o protocolo HTTPS. |
| recurso | string | Obrigatório. Especifica o recurso que será monitorado para detectar alterações. Não incluir a URL base (`https://graph.microsoft.com/beta/`). |
| expirationDateTime | DateTimeOffset | Obrigatório. Especifica a data e a hora em que a assinatura do webhook expira. O horário está em UTC e pode ser uma quantidade de tempo desde a criação da assinatura que varia para o recurso assinado.  Confira na tabela abaixo o tempo máximo permitido para a assinatura. |
| clientState | string | Opcional. Especifica o valor da propriedade `clientState` enviada pelo serviço em cada notificação. O tamanho máximo é de 255 caracteres. O cliente pode verificar se a notificação foi proveniente do serviço comparando o valor da propriedade `clientState` enviada com a assinatura com o valor da propriedade `clientState` recebida com cada notificação. |
| id | cadeia de caracteres | Identificador exclusivo da assinatura. Somente leitura. |
| ApplicationId | string | Identificador do aplicativo usado para criar a assinatura. Somente leitura. |
| creatorId | cadeia de caracteres | Identificador de usuário ou entidade de serviço que criou a assinatura. Se o aplicativo usado delegada permissões para criar a assinatura, esse campo contém a id do usuário que entrou no aplicativo chamado em nome dele. Se o aplicativo usou permissões do aplicativo, esse campo contém a id da entidade de serviço correspondente ao aplicativo. Somente leitura. |

## <a name="maximum-length-of-subscription-per-resource-type"></a>Tamanho máximo da assinatura por tipo de recurso

| Recurso            | Tempo de Expiração Máximo  |
|:--------------------|:-------------------------|
| Usuário, grupo, outros recursos de diretório   | 4230 minutos (em 3 dias)    |
| Email                | 4230 minutos (em 3 dias)    |
| Calendário            | 4230 minutos (em 3 dias)    |
| Contatos            | 4230 minutos (em 3 dias)    |
| Conversas em grupo | 4230 minutos (em 3 dias)    |
| Itens raiz de unidade    | 4230 minutos (em 3 dias)    |
| Alertas de segurança     | 43200 minutos (em 30 dias )  |

> **Observação:** Os aplicativos existentes e os novos aplicativos não devem ultrapassar o valor suportado. No futuro, as solicitações para criar ou renovar uma assinatura além do valor máximo falharão.

## <a name="relationships"></a>Relações

Nenhum

## <a name="methods"></a>Métodos

| Método | Tipo de retorno | Descrição |
|:-------|:------------|:------------|
| [Criar assinatura](../api/subscription-post-subscriptions.md) | [subscription](subscription.md) | Assina um aplicativo de escuta para receber notificações quando dados do Microsoft Graph são alterados. |
| [Atualizar assinatura](../api/subscription-update.md) | [subscription](subscription.md) | Renovar uma assinatura atualizando seu tempo de expiração. |
| [Listar de assinaturas](../api/subscription-list.md) | [assinatura](subscription.md) | Lista assinaturas ativas. |
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
  "suppressions": []
}
-->
