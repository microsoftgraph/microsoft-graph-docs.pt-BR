---
title: tipo de recurso de assinatura
description: 'Uma assinatura que permite a um aplicativo cliente receber notificações sobre alterações de dados no Microsoft Graph. Atualmente, as assinaturas estão habilitadas para os seguintes recursos:'
ms.localizationpriority: medium
author: Jumaodhiss
doc_type: resourcePageType
ms.prod: change-notifications
ms.openlocfilehash: 0e00ce027cee043157e6cd4e7417445c5398b279
ms.sourcegitcommit: c900d22144429ac7aecae3355a4cdc1987cc4234
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/13/2021
ms.locfileid: "61424347"
---
# <a name="subscription-resource-type"></a>tipo de recurso de assinatura

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma assinatura que permite a um aplicativo cliente receber notificações sobre alterações de dados no Microsoft Graph. Atualmente, as assinaturas estão habilitadas para os seguintes recursos. 

> **Observação** Assinaturas marcadas com um asterisco (*) são suportadas apenas no ponto de extremidade beta.

- Um [alert][] da API de Segurança do Microsoft Graph.
- Uma [callRecord][] produzida após uma chamada ou uma reunião no Microsoft Teams.
- Um [canal](./channel.md) em Microsoft Teams.*
- Um [chat](./chat.md) em Microsoft Teams.*
- Um [chatMessage][] enviado por meio de equipes ou canais no Microsoft Teams.
- Uma [conversation][] em um grupo do Microsoft 365.
- Um [conversationMember](./conversationmember.md) em uma equipe, canal ou chat em Microsoft Teams.*
- Conteúdo da hierarquia de uma pasta raiz [driveItem][] no OneDrive for Business ou de uma pasta raiz ou uma subpasta [driveItem][] no OneDrive pessoal do usuário.
- Um [grupo][] no Azure Active Directory.
- Uma [list][] em um [site][] do SharePoint.
- Uma [message][], [event][] ou [contact][] no Outlook.
- A [presença][] de um usuário no Microsoft Teams.*
- Uma [equipe](./team.md) em Microsoft Teams.*
- Uma [printer][] (quando um trabalho de impressão para a impressora chegar ao estado JobFetchable – pronto para ser buscado para impressão) e uma [PrintTaskDefinition][] em Impressão Universal. Para saber mais, confira [Inscrever-se para alterar notificações de APIs de impressão na nuvem](/graph/universal-print-webhook-notifications).
- Uma [baseTask][] de um usuário em Microsoft To Do.*
- Um [usuário][] no Azure Active Directory.

Para obter os valores de caminho de recurso possíveis para cada recurso com suporte, consulte [Usar a API do Microsoft Graph para obter notificações de alteração](webhooks.md).

## <a name="methods"></a>Métodos

| Método | Tipo de retorno | Descrição |
|:-------|:------------|:------------|
| [Criar assinatura](../api/subscription-post-subscriptions.md) | [assinatura](subscription.md) | Assina um aplicativo de escuta para receber notificações sobre alterações nos dados do Microsoft Graph. |
| [Atualizar assinatura](../api/subscription-update.md) | [subscription](subscription.md) | Renove uma assinatura atualizando seu tempo de expiração. |
| [Listar de assinaturas](../api/subscription-list.md) | [assinatura](subscription.md) | Lista assinaturas ativas. |
| [Obter assinatura](../api/subscription-get.md) | [subscription](subscription.md) | Ler propriedades e relações do objeto subscription. |
| [Excluir assinatura](../api/subscription-delete.md) | Nenhuma | Excluir um objeto subscription. |

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição | Recursos com Suporte |
|:---------|:-----|:------------|:--------------|
| ApplicationId | cadeia de caracteres | Identificador do aplicativo utilizado para criar a assinatura. Somente leitura. | Todos |
| changeType | string | Indica qual é o tipo de alteração no recurso inscrito que irá emitir uma notificação de alteração. Os valores com suporte são: `created`, `updated`, `deleted`. Vários valores podem ser combinados usando uma lista separada por vírgula. Obrigatório. <br><br>Observação: As notificações de alteração de lista e item raiz da unidade suportam apenas o `updated` changeType. Suporte para notificações de alteração de usuário e grupo `updated` e `deleted` changeType. | Todos |
| clientState | string | Especifica o valor da propriedade **clientState** enviada pelo serviço em cada notificação de alteração. O tamanho máximo é de 255 caracteres. O cliente pode verificar se a notificação de alteração veio do serviço comparando o valor da propriedade **clientState** enviada com a assinatura com o valor da propriedade **clientState** recebida com cada notificação de alteração. Opcional. | Todos |
| creatorId | cadeia de caracteres | Identificador de usuário ou entidade de serviço que criou a assinatura. Se o aplicativo usou permissões delegadas para criar a assinatura, este campo conterá a ID do usuário inscreva o aplicativo chamado em nome de. Se o aplicativo usou permissões de aplicativo, este campo contém a ID da entidade de serviço correspondente ao aplicativo. Somente leitura. | Todos |
| encryptionCertificate | cadeia de caracteres | Uma representação codificada em Base64 de um certificado com uma chave pública usada para criptografar os dados de recursos nas notificações de alteração. Opcional. Obrigatório quando **includeResourceData** é verdadeiro. | Todos |
| encryptionCertificateId | cadeia de caracteres | Um identificador personalizado fornecido pelo aplicativo para ajudar a identificar o certificado necessário para descriptografar os dados do recurso. Opcional. Obrigatório quando **includeResourceData** é verdadeiro. | Todos |
| expirationDateTime | DateTimeOffset | Especifica a data e a hora em que a assinatura do webhook expira. O horário está em UTC e pode ser uma quantidade de tempo desde a criação da assinatura que varia para o recurso assinado.  Confira na tabela abaixo o tempo máximo permitido para a assinatura. Obrigatório. | Todos |
| id | string | Identificador exclusivo da assinatura. Somente leitura. | Todos |
| includeResourceData | Booleano | Quando definido como `true`, alterar as notificações [inclui dados de recurso](/graph/webhooks-with-resource-data) (como o conteúdo de uma mensagem de bate-papo). Opcional. | Todos |
| latestSupportedTlsVersion | string | Especifica a versão mais recente do protocolo TLS que o ponto de extremidade, especificado por **notificationUrl**, é compatível. Os valores possíveis são: `v1_0`, `v1_1`, `v1_2`, `v1_3`. </br></br>Para os assinantes cujo ponto de extremidade de notificação suporta uma versão menor que a versão recomendada atualmente (TLS 1.2), especificar essa propriedade por uma [linha do tempo](https://developer.microsoft.com/graph/blogs/microsoft-graph-subscriptions-deprecating-tls-1-0-and-1-1/) definida, permite o uso temporário da versão preterida do TLS antes de concluir a atualização para o TLS 1.2. Para esses assinantes, não definir essa propriedade pela linha do tempo resultaria em uma falha nas operações da assinatura. </br></br>Para os assinantes cujo ponto de extremidade já tem suporte ao TLS 1.2, a configuração dessa propriedade é opcional. Nesses casos, o Microsoft Graph padroniza a propriedade como `v1_2`. | Todos |
| lifecycleNotificationUrl | string | A URL do ponto de extremidade que recebe notificações do ciclo de vida, incluindo notificações de `subscriptionRemoved` e `missed`. Esta URL deve fazer uso do protocolo HTTPS. Opcional. <br><br>[Leia mais](/graph/webhooks-lifecycle) sobre como os recursos do Outlook usam notificações do ciclo de vida. | Todos |
| notificationContentType | cadeia de caracteres | Tipo de conteúdo desejado para as notificações de alteração do MS Graph para os tipos de recursos com suporte. O tipo de conteúdo padrão é o tipo de conteúdo "aplicativo/json". | Todos |
| notificationQueryOptions | cadeia de caracteres | Opções de Consulta OData para especificar o valor do recurso de destino. Os clientes recebem notificações quando o recurso atinge ao estado correspondente às opções de consulta aqui fornecidas. Com essa nova propriedade na carga de criação de assinatura, juntamente com todas as propriedades existentes, os Webhooks enviarão notificações sempre que um recurso atingir o estado desejado mencionado na propriedade notificationQueryOptions. Por exemplo, quando o trabalho de impressão for concluído, quando o valor de uma propriedade `isFetchable` do recurso de impressão se tornar verdadeiro etc. | [Serviço de Impressão Universal](/graph/universal-print-webhook-notifications) |
| notificationUrl | cadeia de caracteres | A URL do ponto de extremidade que recebe as notificações de alteração. Esta URL deve fazer uso do protocolo HTTPS. Obrigatório. | Todos |
| recurso | string | Especifica o recurso que será monitorado para detectar alterações. Não incluir a URL base (`https://graph.microsoft.com/beta/`). Consulte os possíveis valores do [caminho](webhooks.md) do recurso de cada recurso suportado. Obrigatório. | Todos |

### <a name="maximum-length-of-subscription-per-resource-type"></a>Tamanho máximo da assinatura por tipo de recurso

| Resource            | Tempo de expiração máximo  |
|:--------------------|:-------------------------|
| **Alerta** de segurança     | 43200 minutos (em 30 dias )  |
| Teams **callRecord**    | 4230 minutos (em 3 dias)  |
| **Canal** do Teams    | 60 minutos (1 hora)  |
| **Chat** do Teams | 60 minutos (1 hora) |
| Teams **chatMessage**    | 60 minutos (1 hora)  |
| **conversationMember** do Teams    | 60 minutos (1 hora)  |
| Equipe do **Teams**    | 60 minutos (1 hora)  |
| **Conversa** em grupo | 4230 minutos (em 3 dias)    |
| OneDrive **driveItem**    | 42.300 minutos (menos de 30 dias)    |
| **Lista** do Microsoft Office SharePoint Online    | 42.300 minutos (menos de 30 dias)    |
| Outlook **mensagem**, **evento**, **contato**              | 4230 minutos (em 3 dias)    |
| **usuário**, **grupo**, outros recursos de diretório   | 41760 minutos (menos de 29 dias)    |
| **presence**        | 60 minutos (1 hora) |
| Imprimir **printer** | 4230 minutos (em 3 dias)    |
| Imprimir **printTaskDefinition** | 4230 minutos (em 3 dias)    |
| **baseTask**              | 4230 minutos (em 3 dias)    |


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
[baseTask]: ./basetask.md

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


