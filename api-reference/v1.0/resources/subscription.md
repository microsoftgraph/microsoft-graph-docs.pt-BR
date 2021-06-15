---
title: tipo de recurso de assinatura
description: 'Uma assinatura que permite a um aplicativo cliente receber notificações sobre alterações de dados no Microsoft Graph. Atualmente, as assinaturas estão habilitadas para os seguintes recursos:'
localization_priority: Priority
author: Jumaodhiss
ms.prod: change-notifications
doc_type: resourcePageType
ms.openlocfilehash: c47c4d7df11599a5983f5610ef3bfd29c80eee5b
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/12/2021
ms.locfileid: "52911288"
---
# <a name="subscription-resource-type"></a>tipo de recurso de assinatura

Namespace: microsoft.graph

Uma assinatura que permite a um aplicativo cliente receber notificações sobre alterações de dados no Microsoft Graph. Atualmente, as assinaturas estão habilitadas para os seguintes recursos:

- Um [alert][] da API de Segurança do Microsoft Graph.
- Uma [callRecord][] produzida após uma chamada ou uma reunião no Microsoft Teams.
- Um [chatMessage][] enviado por meio de equipes ou canais no Microsoft Teams.
- Uma [conversation][] em um grupo do Microsoft 365.
- Conteúdo da hierarquia de uma pasta raiz [driveItem][] no OneDrive for Business ou de uma pasta raiz ou uma subpasta [driveItem][] no OneDrive pessoal do usuário.
- Uma [list][] em um [site][] do SharePoint.
- Uma [message][], [event][] ou [contact][] no Outlook.
- Uma [printer][] (quando um trabalho de impressão para a impressora chegar ao estado JobFetchable – pronto para ser buscado para impressão) e uma [PrintTaskDefinition][] em Impressão Universal. Para saber mais, confira [Inscrever-se para alterar notificações de APIs de impressão na nuvem](/graph/universal-print-webhook-notifications).
- Um [user][] ou [group][] no Azure Active Directory.

Consulte [usar o Microsoft Graph API para obter notificações de alteração](webhooks.md) dos possíveis valores de caminho de recurso de cada recurso suportado.

## <a name="methods"></a>Métodos

| Método | Tipo de retorno | Descrição |
|:-------|:------------|:------------|
| [Criar assinatura](../api/subscription-post-subscriptions.md) | [assinatura](subscription.md) | Assina um aplicativo de escuta para receber notificações sobre alterações nos dados do Microsoft Graph. |
| [Atualizar assinatura](../api/subscription-update.md) | [subscription](subscription.md) | Renova uma assinatura atualizando seu tempo de expiração. |
| [Listar de assinaturas](../api/subscription-list.md) | [assinatura](subscription.md) | Lista assinaturas ativas. |
| [Obter assinatura](../api/subscription-get.md) | [subscription](subscription.md) | Lê as propriedades e as relações do objeto subscription. |
| [Excluir assinatura](../api/subscription-delete.md) | Nenhuma | Exclui um objeto assinatura. |

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição | Recursos com Suporte |
|:---------|:-----|:------------|:--------------|
| changeType | string | Obrigatório. Indica qual é o tipo de alteração no recurso inscrito que irá emitir uma notificação de alteração. Os valores com suporte são: `created`, `updated`, `deleted`. Vários valores podem ser combinados usando uma lista separada por vírgula.<br><br>Observação: As notificações de alteração de lista e item raiz da unidade suportam apenas o `updated` changeType. Suporte para notificações de alteração de usuário e grupo `updated` e `deleted` changeType. | Todos |
| notificationUrl | cadeia de caracteres | Obrigatório. O URL do ponto de extremidade que receberá as notificações de alteração. Este URL deve fazer uso do protocolo HTTPS. | Todos |
| lifecycleNotificationUrl | string | A URL do ponto de extremidade que recebe notificações do ciclo de vida, incluindo notificações de `subscriptionRemoved` e `missed`. Esta URL deve fazer uso do protocolo HTTPS. Opcional. <br><br>[Leia mais](/graph/webhooks-lifecycle) sobre como os recursos do Outlook usam notificações do ciclo de vida. | Todos |
| recurso | string | Obrigatório. Especifica o recurso que será monitorado para detectar alterações. Não incluir a URL base (`https://graph.microsoft.com/v1.0/`). Consulte os possíveis valores do [caminho](webhooks.md) do recurso de cada recurso suportado.| Todos |
| expirationDateTime | [dateTime](https://tools.ietf.org/html/rfc3339) | Obrigatório. Especifica a data e hora em que a assinatura do webhook expira. O horário está em UTC e pode ser uma quantidade de tempo desde a criação da assinatura que varia de acordo com o recurso assinado. Consulte a tabela abaixo para obter a duração máxima da assinatura com suporte. | Todos |
| clientState | string | Opcional. Especifica o valor da propriedade `clientState` enviada pelo serviço em cada notificação de alteração. O comprimento máximo é de 128 caracteres. O cliente pode verificar se a notificação de alteração veio do serviço pela comparação do valor da propriedade `clientState` enviada com a assinatura com o valor da propriedade `clientState` recebida contendo cada notificação de alteração. | Todos |
| id | string | Identificador exclusivo da assinatura. Somente leitura. | Todos |
| ApplicationId | cadeia de caracteres | Identificador do aplicativo utilizado para criar a assinatura. Somente leitura. | Todos |
| creatorId | cadeia de caracteres | Identificador de usuário ou entidade de serviço que criou a assinatura. Se o aplicativo usado delegada permissões para criar a assinatura, esse campo contém a id do usuário que entrou no aplicativo chamado em nome dele. Se o aplicativo usou permissões do aplicativo, esse campo contém a id da entidade de serviço correspondente ao aplicativo. Somente leitura. | Todos |
| includeResourceData | Booleano | Quando definido como `true`, alterar as notificações [inclui dados de recurso](/graph/webhooks-with-resource-data) (como o conteúdo de uma mensagem de bate-papo). Opcional. | Todos |
| encryptionCertificate | cadeia de caracteres | Uma representação codificada em Base64 de um certificado com uma chave pública usada para criptografar os dados de recursos nas notificações de alteração. Opcional. Obrigatório quando **includeResourceData** é verdadeiro. | Todos |
| encryptionCertificateId | cadeia de caracteres | Um aplicativo personalizado forneceu um identificador para ajudar a identificar o certificado necessário para decodificar os dados dos recursos. Opcional.| Todos |
| latestSupportedTlsVersion | Cadeia de caracteres | Especifica a versão mais recente do protocolo TLS que o ponto de extremidade, especificado por **notificationUrl**, é compatível. Os valores possíveis são: `v1_0`, `v1_1`, `v1_2`, `v1_3`. </br></br>Para os assinantes cujo ponto de extremidade de notificação suporta uma versão menor que a versão recomendada atualmente (TLS 1.2), especificar essa propriedade por uma [linha do tempo](https://developer.microsoft.com/graph/blogs/microsoft-graph-subscriptions-deprecating-tls-1-0-and-1-1/) definida, permite o uso temporário da versão preterida do TLS antes de concluir a atualização para o TLS 1.2. Para esses assinantes, não definir essa propriedade pela linha do tempo resultaria em uma falha nas operações da assinatura. </br></br>Para os assinantes cujo ponto de extremidade já tem suporte ao TLS 1.2, a configuração dessa propriedade é opcional. Nesses casos, o Microsoft Graph padroniza a propriedade como `v1_2`. | Todos |
| notificationContentType | cadeia de caracteres | Tipo de conteúdo desejado para as notificações de alteração do MS Graph para os tipos de recursos com suporte. O tipo de conteúdo padrão é o tipo de conteúdo "aplicativo/json". | Todos |
| notificationQueryOptions | cadeia de caracteres | Opções de Consulta OData para especificar o valor do recurso de destino. Os clientes recebem notificações quando o recurso atinge ao estado correspondente às opções de consulta aqui fornecidas. Com essa nova propriedade na carga de criação de assinatura, juntamente com todas as propriedades existentes, os Webhooks enviarão notificações sempre que um recurso atingir o estado desejado mencionado na propriedade notificationQueryOptions. Por exemplo, quando o trabalho de impressão for concluído, quando o valor de uma propriedade `isFetchable` do recurso de impressão se tornar verdadeiro etc. | [Serviço de Impressão Universal](/graph/universal-print-webhook-notifications) |

### <a name="maximum-length-of-subscription-per-resource-type"></a>Tamanho máximo da assinatura por tipo de recurso

| Resource            | Tempo de expiração máximo  |
|:--------------------|:-------------------------|
| **Alerta** de segurança     | 43200 minutos (em 30 dias )  |
| Teams **callRecord**    | 4230 minutos (em 3 dias)  |
| Teams **chatMessage**    | 60 minutos (1 hora)  |
| **Conversa** em grupo | 4230 minutos (em 3 dias)    |
| OneDrive **driveItem**    | 42.300 minutos (menos de 30 dias)    |
| **Lista** do Microsoft Office SharePoint Online    | 42.300 minutos (menos de 30 dias)    |
| Outlook **mensagem**, **evento**, **contato**              | 4230 minutos (em 3 dias)    |
| **usuário**, **grupo**, outros recursos de diretório   | 4230 minutos (em 3 dias)    |
| Imprimir **printer** | 4230 minutos (em 3 dias)    |
| Imprimir **printTaskDefinition** | 4230 minutos (em 3 dias)    |


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
  "expirationDateTime": "String (timestamp)",
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
[impressora]: ./printer.md
[printTaskDefinition]: ./printtaskdefinition.md

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "subscription resource",
  "keywords": "",
  "section": "documentation",
  "tocPath&quot;: &quot;"
}-->

