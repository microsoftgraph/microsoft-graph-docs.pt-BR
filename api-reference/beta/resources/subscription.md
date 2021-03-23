---
title: tipo de recurso de assinatura
description: 'Uma assinatura que permite a um aplicativo cliente receber notificações sobre alterações de dados no Microsoft Graph. Atualmente, as assinaturas estão habilitadas para as seguintes coleções de recursos:'
localization_priority: Normal
author: Jumaodhiss
doc_type: resourcePageType
ms.prod: change-notifications
ms.openlocfilehash: 81bb0e1b914a547b8c9fef55b446158069b77b23
ms.sourcegitcommit: 74a1fb3874e04c488e1b87dcee80d76cc586c1f3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51030971"
---
# <a name="subscription-resource-type"></a>tipo de recurso de assinatura

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma assinatura que permite a um aplicativo cliente receber notificações sobre alterações de dados no Microsoft Graph. Atualmente, as assinaturas estão habilitadas para as seguintes coleções de recursos:

- Um [alerta][] da API de Segurança do Microsoft Graph.
- Um [callRecord][] produzido após uma chamada ou reunião no Microsoft Teams.
- Um [chatMessage enviado][] por meio de equipes ou canais no Microsoft Teams.
- Uma [conversa][] em um grupo do Microsoft 365.
- Conteúdo na hierarquia de uma pasta raiz [driveItem][] no OneDrive for Business ou de uma pasta raiz ou [driveItem][] de subpasta no OneDrive pessoal de um usuário.
- Uma [lista][] em um [site][]do SharePoint.
- Uma [mensagem][], [evento][]ou [contato][] no Outlook.
- A [presença][] de um usuário no Microsoft Teams.
- Um [usuário][] ou [grupo][] no Azure Active Directory.
- Uma [impressora][] (quando um trabalho de impressão para a impressora chega ao estado JobFetchable - pronto para ser buscado para impressão) e uma [printTaskDefinition][] em Impressão Universal. Para obter mais informações, consulte [Subscribe to change notifications from cloud printing APIs](https://docs.microsoft.com/en-us/graph/universal-print-webhook-notifications).
- Um [todoTask][] de um usuário no Microsoft To Do.

Consulte [usar o Microsoft Graph API para obter notificações de alteração](webhooks.md) dos possíveis valores de caminho de recurso de cada recurso suportado.

## <a name="methods"></a>Métodos

| Método | Tipo de retorno | Descrição |
|:-------|:------------|:------------|
| [Criar assinatura](../api/subscription-post-subscriptions.md) | [assinatura](subscription.md) | Assina um aplicativo de escuta para receber notificações sobre alterações nos dados do Microsoft Graph. |
| [Atualizar assinatura](../api/subscription-update.md) | [subscription](subscription.md) | Renove uma assinatura atualizando seu tempo de expiração. |
| [Listar de assinaturas](../api/subscription-list.md) | [assinatura](subscription.md) | Lista assinaturas ativas. |
| [Obter assinatura](../api/subscription-get.md) | [subscription](subscription.md) | Ler propriedades e relações do objeto subscription. |
| [Excluir assinatura](../api/subscription-delete.md) | Nenhuma | Excluir um objeto subscription. |

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição | Recursos suportados |
|:---------|:-----|:------------|:--------------|
| changeType | cadeia de caracteres | Indica qual é o tipo de alteração no recurso inscrito que irá emitir uma notificação de alteração. Os valores com suporte são: `created`, `updated`, `deleted`. Vários valores podem ser combinados usando uma lista separada por vírgula. Obrigatório. <br><br>Observação: As notificações de alteração de lista e item raiz da unidade suportam apenas o `updated` changeType. Suporte para notificações de alteração de usuário e grupo `updated` e `deleted` changeType. | Todos |
| notificationUrl | cadeia de caracteres | A URL do ponto de extremidade que recebe as notificações de alteração. Esta URL deve usar o protocolo HTTPS. Obrigatório. | Todos |
| lifecycleNotificationUrl | cadeia de caracteres | A URL do ponto de extremidade que recebe notificações de ciclo de vida, incluindo `subscriptionRemoved` e `missed` notificações. Esta URL deve usar o protocolo HTTPS. Opcional. <br><br>[Leia mais sobre](/graph/webhooks-lifecycle) como os recursos do Outlook usam notificações de ciclo de vida. | Todos |
| recurso | cadeia de caracteres | Especifica o recurso que será monitorado para detectar alterações. Não incluir a URL base (`https://graph.microsoft.com/beta/`). Consulte os possíveis valores do [caminho](webhooks.md) do recurso de cada recurso suportado. Obrigatório. | Todos |
| expirationDateTime | DateTimeOffset | Especifica a data e a hora em que a assinatura do webhook expira. O horário está em UTC e pode ser uma quantidade de tempo desde a criação da assinatura que varia para o recurso assinado.  Confira na tabela abaixo o tempo máximo permitido para a assinatura. Obrigatório. | Todos |
| clientState | string | Especifica o valor da propriedade **clientState** enviada pelo serviço em cada notificação de alteração. O tamanho máximo é de 255 caracteres. O cliente pode verificar se a notificação de alteração veio do serviço comparando o valor da propriedade **clientState** enviada com a assinatura com o valor da propriedade **clientState** recebida com cada notificação de alteração. Opcional. | Todos |
| id | string | Identificador exclusivo da assinatura. Somente leitura. | Todos |
| ApplicationId | cadeia de caracteres | Identificador do aplicativo usado para criar a assinatura. Somente leitura. | Todos |
| creatorId | cadeia de caracteres | Identificador de usuário ou entidade de serviço que criou a assinatura. Se o aplicativo usou permissões delegadas para criar a assinatura, este campo conterá a ID do usuário inscreva o aplicativo chamado em nome de. Se o aplicativo usou permissões de aplicativo, este campo contém a ID da entidade de serviço correspondente ao aplicativo. Somente leitura. | Todos |
| includeResourceData | Booleano | Quando definido como `true`, alterar as notificações [inclui dados de recurso](/graph/webhooks-with-resource-data) (como o conteúdo de uma mensagem de bate-papo). Opcional. | Todos |
| encryptionCertificate | cadeia de caracteres | Uma representação codificada em Base64 de um certificado com uma chave pública usada para criptografar os dados de recursos nas notificações de alteração. Opcional. Obrigatório quando **includeResourceData** é verdadeiro. | Todos |
| encryptionCertificateId | cadeia de caracteres | Um identificador personalizado fornecido pelo aplicativo para ajudar a identificar o certificado necessário para descriptografar os dados do recurso. Opcional. Obrigatório quando **includeResourceData** é verdadeiro. | Todos |
| latestSupportedTlsVersion | cadeia de caracteres | Especifica a versão mais recente do protocolo TLS que o ponto de extremidade, especificado por **notificationUrl**, é compatível. Os valores possíveis são: `v1_0`, `v1_1`, `v1_2`, `v1_3`. </br></br>Para os assinantes cujo ponto de extremidade de notificação suporta uma versão menor que a versão recomendada atualmente (TLS 1.2), especificar essa propriedade por uma [linha do tempo](https://developer.microsoft.com/graph/blogs/microsoft-graph-subscriptions-deprecating-tls-1-0-and-1-1/) definida, permite o uso temporário da versão preterida do TLS antes de concluir a atualização para o TLS 1.2. Para esses assinantes, não definir essa propriedade pela linha do tempo resultaria em uma falha nas operações da assinatura. </br></br>Para os assinantes cujo ponto de extremidade já tem suporte ao TLS 1.2, a configuração dessa propriedade é opcional. Nesses casos, o Microsoft Graph padroniza a propriedade como `v1_2`. | Todos |
| notificationContentType | cadeia de caracteres | Tipo de conteúdo desejado para notificações de alteração do MS Graph para tipos de recursos com suporte. O tipo de conteúdo padrão é o tipo de conteúdo "application/json". | Todos |
| notificationQueryOptions | cadeia de caracteres | Opções de consulta OData para especificar o valor do recurso de direcionamento. Os clientes recebem notificações quando o recurso atinge o estado correspondente às opções de consulta fornecidas aqui. Com essa nova propriedade na carga de criação de assinatura juntamente com todas as propriedades existentes, os Webhooks fornecerão notificações sempre que um recurso atingir o estado desejado mencionado na propriedade notificationQueryOptions por exemplo, quando o trabalho de impressão for concluído, quando um valor de propriedade de recurso de trabalho de impressão se tornar `isFetchable` verdadeiro etc. | [Serviço de Impressão Universal](https://docs.microsoft.com/en-us/graph/universal-print-webhook-notifications) |

### <a name="maximum-length-of-subscription-per-resource-type"></a>Tamanho máximo da assinatura por tipo de recurso

| Resource            | Tempo de expiração máximo  |
|:--------------------|:-------------------------|
| **Alerta** de segurança     | 43200 minutos (em 30 dias )  |
| Teams **callRecord**    | 4230 minutos (em 3 dias)  |
| Teams **chatMessage**    | 60 minutos (1 hora)  |
| **Conversa** em grupo | 4230 minutos (em 3 dias)    |
| OneDrive **driveItem**    | 4230 minutos (em 3 dias)    |
| **Lista** do Microsoft Office SharePoint Online    | 4230 minutos (em 3 dias)    |
| Outlook **mensagem**, **evento**, **contato**              | 4230 minutos (em 3 dias)    |
| **usuário**, **grupo**, outros recursos de diretório   | 4230 minutos (em 3 dias)    |
| **presence**        | 60 minutos (1 hora) |
| Impressora **de impressão** | 4230 minutos (em 3 dias)    |
| Imprimir **printTaskDefinition** | 4230 minutos (em 3 dias)    |
| **todoTask**              | 4230 minutos (em 3 dias)    |


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
  "lifecycleNotificationUrl": "string",
  "resource": "string",
  "applicationId" : "string",
  "expirationDateTime": "string (timestamp)",
  "id": "string (identifier)",
  "clientState": "string",
  "creatorId": "string",
  "includeResourceData": "boolean",
  "encryptionCertificate": "string",
  "encryptionCertificateId": "string",
  "latestSupportedTlsVersion": "string",
  "notificationContentType": "string",
  "notificationQueryOptions": "string"
}
```

[contato]: ./contact.md
[conversa]: ./conversation.md
[driveItem]: ./driveitem.md
[list]: ./list.md
[site]: ./site.md
[event]: ./event.md
[group]: ./group.md
[message]: ./message.md
[user]: ./user.md
[alert]: ./alert.md
[chatMessage]: ./chatmessage.md
[callRecord]: ./callrecords-callrecord.md
[presence]: ./presence.md
[impressora]: ./printer.md
[printTaskDefinition]: ./printtaskdefinition.md
[todoTask]: ./todotask.md

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


