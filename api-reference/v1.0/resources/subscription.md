---
title: tipo de recurso de assinatura
description: 'Uma assinatura permite que um aplicativo cliente receba notificações sobre dados no Microsoft Graph. Atualmente, as assinaturas estão habilitadas para as seguintes coleções de recursos:'
localization_priority: Priority
author: baywet
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: a490257ccc1ba17e7e425c24126c24689c612a9b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533600"
---
# <a name="subscription-resource-type"></a>tipo de recurso de assinatura

Namespace: microsoft.graph

Uma assinatura permite que um aplicativo cliente receba notificações sobre dados no Microsoft Graph. Atualmente, as assinaturas estão habilitadas para as seguintes coleções de recursos:

- Um [alerta][] do Microsoft Graph Security API
- Um [conversa][] de um grupo do Office 365
- Conteúdo da hierarquia de uma pasta raiz [driveItem][] no OneDrive for Business ou de uma pasta raiz ou uma subpasta [driveItem][] no OneDrive pessoal do usuário
- Uma [mensagem][], [evento][] ou [contato][] no Outlook
- Um [usuário][] ou [grupo][] no Azure Active Directory

Consulte [usar o Microsoft Graph API para obter notificações de alteração](webhooks.md) dos possíveis valores de caminho de recurso de cada recurso suportado.

## <a name="methods"></a>Métodos

| Método | Tipo de retorno | Descrição |
|:-------|:------------|:------------|
| [Criar assinatura](../api/subscription-post-subscriptions.md) | [subscription](subscription.md) | Assina um aplicativo de escuta para receber notificações quando dados do Microsoft Graph são alterados. |
| [Atualizar assinatura](../api/subscription-update.md) | [subscription](subscription.md) | Renova uma assinatura atualizando seu tempo de expiração. |
| [Listar de assinaturas](../api/subscription-list.md) | [assinatura](subscription.md) | Lista assinaturas ativas. |
| [Obter assinatura](../api/subscription-get.md) | [subscription](subscription.md) | Lê as propriedades e as relações do objeto subscription. |
| [Excluir assinatura](../api/subscription-delete.md) | Nenhuma | Exclui um objeto assinatura. |

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------|:-----|:------------|
| changeType | cadeia de caracteres | Obrigatório. Indica o tipo de alteração no recurso inscrito que gerará uma notificação. Os valores com suporte são: `created`, `updated`, `deleted`. Vários valores podem ser combinados usando uma lista separada por vírgula.<br><br>Observação: As notificações do item na raiz da unidade suportam somente `updated` changeType. Notificações de grupos e usuário suportam `updated` e `deleted` changeType. |
| notificationUrl | cadeia de caracteres | Obrigatório. A URL do ponto de extremidade que receberá as notificações. Esta URL deve usar o protocolo HTTPS. |
| recurso | cadeia de caracteres | Obrigatório. Especifica o recurso que será monitorado para detectar alterações. Não incluir a URL base (`https://graph.microsoft.com/v1.0/`). Consulte os possíveis valores do [caminho](webhooks.md) do recurso de cada recurso suportado.|
| expirationDateTime | [dateTime](https://tools.ietf.org/html/rfc3339) | Obrigatório. Especifica a data e a hora em que a assinatura do webhook expira. O horário está em UTC e pode ser uma quantidade de tempo desde a criação da assinatura que varia para o recurso assinado.  Confira na tabela abaixo o tempo máximo permitido para a assinatura. |
| clientState | string | Opcional. Especifica o valor da propriedade `clientState` enviada pelo serviço em cada notificação. O comprimento máximo é de 128 caracteres. O cliente pode verificar se a notificação foi proveniente do serviço comparando o valor da propriedade `clientState` enviada com a assinatura com o valor da propriedade `clientState` recebida com cada notificação. |
| id | string | Identificador exclusivo da assinatura. Somente leitura. |
| ApplicationId | cadeia de caracteres | Identificador do aplicativo usado para criar a assinatura. Somente leitura. |
| creatorId | cadeia de caracteres | Identificador de usuário ou entidade de serviço que criou a assinatura. Se o aplicativo usado delegada permissões para criar a assinatura, esse campo contém a id do usuário que entrou no aplicativo chamado em nome dele. Se o aplicativo usou permissões do aplicativo, esse campo contém a id da entidade de serviço correspondente ao aplicativo. Apenas leitura. |
| latestSupportedTlsVersion | Cadeia de caracteres | Especifica a versão mais recente do protocolo TLS que o ponto de extremidade, especificado por **notificationUrl**, é compatível. Os valores possíveis são: `v1_0`, `v1_1`, `v1_2`, `v1_3`. </br></br>Para os assinantes cujo ponto de extremidade de notificação suporta uma versão menor que a versão recomendada atualmente (TLS 1.2), especificar essa propriedade por uma [linha do tempo](https://developer.microsoft.com/graph/blogs/microsoft-graph-subscriptions-deprecating-tls-1-0-and-1-1/) definida, permite o uso temporário da versão preterida do TLS antes de concluir a atualização para o TLS 1.2. Para esses assinantes, não definir essa propriedade pela linha do tempo resultaria em uma falha nas operações da assinatura. </br></br>Para os assinantes cujo ponto de extremidade já tem suporte ao TLS 1.2, a configuração dessa propriedade é opcional. Nesses casos, o Microsoft Graph padroniza a propriedade como `v1_2`. |

### <a name="maximum-length-of-subscription-per-resource-type"></a>Tamanho máximo da assinatura por tipo de recurso

| Resource            | Tempo de expiração máximo  |
|:--------------------|:-------------------------|
| Usuário, grupo, outros recursos de diretório   | 4230 minutos (em 3 dias)    |
| Correio                | 4230 minutos (em 3 dias)    |
| Calendário            | 4230 minutos (em 3 dias)    |
| Contatos            | 4230 minutos (em 3 dias)    |
| Conversas em grupo | 4230 minutos (em 3 dias)    |
| Itens raiz de unidade    | 4230 minutos (em 3 dias)    |
| Alertas de segurança     | 43200 minutos (em 30 dias )  |

> **Observação:** Os aplicativos existentes e os novos aplicativos não devem ultrapassar o valor suportado. No futuro, as solicitações para criar ou renovar uma assinatura além do valor máximo falharão.

## <a name="relationships"></a>Relações

Nenhum

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
  "creatorId": "string",
  "latestSupportedTlsVersion": "string"
}
```

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
