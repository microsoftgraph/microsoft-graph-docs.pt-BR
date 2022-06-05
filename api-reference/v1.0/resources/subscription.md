---
title: tipo de recurso de assinatura
description: 'Uma assinatura que permite a um aplicativo cliente receber notificações sobre alterações de dados no Microsoft Graph. Atualmente, as assinaturas estão habilitadas para os seguintes recursos:'
ms.localizationpriority: high
author: Jumaodhiss
ms.prod: change-notifications
doc_type: resourcePageType
ms.openlocfilehash: 3adc9490dc554344b553de5a0520c66e2f905956
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2022
ms.locfileid: "65900041"
---
# <a name="subscription-resource-type"></a>tipo de recurso de assinatura

Namespace: microsoft.graph

Uma assinatura que permite a um aplicativo cliente receber notificações sobre alterações de dados no Microsoft Graph. Atualmente, as assinaturas estão habilitadas para os seguintes recursos:

- Um [alert][] da API de Segurança do Microsoft Graph.
- Uma [callRecord][] produzida após uma chamada ou uma reunião no Microsoft Teams.
- Um [canal](./channel.md) no Microsoft Teams.
- Um [chat](./chat.md) no Microsoft Teams.
- Um [chatMessage][] enviado por meio de equipes ou canais no Microsoft Teams.
- Uma [conversation][] em um grupo do Microsoft 365.
- Um [conversationMember](./conversationmember.md) em uma equipe ou canal no Microsoft Teams.
- Conteúdo da hierarquia de uma pasta raiz [driveItem][] no OneDrive for Business ou de uma pasta raiz ou uma subpasta [driveItem][] no OneDrive pessoal do usuário.
- Um [grupo][] no Azure Active Directory.
- Uma [list][] em um [site][] do SharePoint.
- Uma [message][], [event][] ou [contact][] no Outlook.
- Uma [impressora][] (quando um trabalho de impressão da impressora chegar ao estado JobFetchable – pronto para ser buscado para impressão) e uma [printTaskDefinition][] na Impressão Universal. Para obter mais informações, consulte [Assinar para alterar as notificações de APIs de impressão na nuvem](/graph/universal-print-webhook-notifications).
- Uma [equipe](./team.md) no Microsoft Teams.
- Uma [todoTask][] de um usuário no Microsoft To Do.*
- Um [usuário][] no Azure Active Directory.

Para obter os valores de caminho de recurso possíveis para cada recurso com suporte, consulte [Usar a API do Microsoft Graph para obter notificações de alteração](webhooks.md). Para saber como usar notificações de ciclo de vida, consulte [Reduzir assinaturas ausentes e alterar notificações](/graph/webhooks-lifecycle).


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
| ApplicationId | Cadeia de caracteres | Opcional. Identificador do aplicativo usado para criar a assinatura. Somente leitura. | Todos |
| changeType | Cadeia de caracteres | Necessário. Indica o tipo de alteração no recurso inscrito que gerará uma alteração de notificação. Os valores com suporte são: `created`, `updated`, `deleted`. Vários valores podem ser combinados usando uma lista separada por vírgula. <br><br>**Observação:** <li> As notificações de alteração de lista e item raiz da unidade dão suporte apenas `updated` changeType. <li>[Usuário](../resources/user.md) e [grupo](../resources/user.md) notificações de alteração dão suporte `updated` e `deleted` changeType. | Todos |
| clientState | String | Opcional. Especifica o valor `clientState` da propriedade enviada pelo serviço em cada alteração de notificação. O comprimento máximo é de 128 caracteres. O cliente pode verificar se a alteração de notificação foi proveniente do serviço comparando o valor `clientState` da propriedade enviada com a assinatura com o valor `clientState` da propriedade recebida com cada alteração de notificação. | Todos |
| creatorId | String | Opcional. Identificador de usuário ou entidade de serviço que criou a assinatura. Se o aplicativo usado delegada permissões para criar a assinatura, esse campo contém a id do usuário que entrou no aplicativo chamado em nome dele. Se o aplicativo usou permissões do aplicativo, esse campo contém a id da entidade de serviço correspondente ao aplicativo. Somente leitura. | Todos |
| encryptionCertificate | Cadeia de caracteres | Opcional. Uma representação codificada em Base64 de um certificado com uma chave pública usada para criptografar os dados dos recursos nas notificações de alteração. Opcional, mas necessário quando **includeResourceData** for `true`. | Todos |
| encryptionCertificateId | String | Opcional. Um aplicativo personalizado forneceu um identificador para ajudar a identificar o certificado necessário para decodificar os dados dos recursos. | Todos |
| expirationDateTime | DateTimeOffset | Obrigatório. Especifique a data e a hora em que a assinatura do Webhook expira. O forário está em UTC e pode ser um período de tempo desde a criação da assinatura que varia de acordo com o recurso assinado. Para obter o período máximo de assinaturas com suporte, consulte [a tabela abaixo](#maximum-length-of-subscription-per-resource-type). | Todos |
| id | Cadeia de caracteres | Opcional. Identificador exclusivo da assinatura. Somente leitura. | Todos |
| includeResourceData | Booleano | Opcional. Quando definido como `true`, alterar as notificações [inclui dados de recurso](/graph/webhooks-with-resource-data) (como o conteúdo de uma mensagem de bate-papo). | Todos |
| latestSupportedTlsVersion | Cadeia de caracteres | Opcional. Especifique a versão mais recente do Protocolo TLS que o ponto de extremidade de notificação, especificado por **notificationUrl**, oferece suporte. Os valores possíveis são: `v1_0`, `v1_1`, `v1_2`, `v1_3`. </br></br>Quanto aos assinantes cujo ponto de extremidade de notificação oferece suporte a uma versão inferior à versão recomendada no momento (TLS 1.2), especificar essa propriedade por um conjunto de [linhas do tempo](https://developer.microsoft.com/graph/blogs/microsoft-graph-subscriptions-deprecating-tls-1-0-and-1-1/) permite que eles usem temporariamente sua versão preterida do TLS antes de concluir a atualização para o TLS 1.2. Para esses assinantes, não definir essa propriedade de acordo com a linha do tempo resultaria em erro nas operações de assinatura.</br></br>Para os assinantes cujo ponto de extremidade já tem suporte ao TLS 1.2, a configuração dessa propriedade é opcional. Nesses casos, o Microsoft Graph padroniza a propriedade como `v1_2`. | Todos |
| lifecycleNotificationUrl | String | Opcional. A URL do ponto de extremidade que recebe notificações do ciclo de vida, incluindo notificações de `subscriptionRemoved` e `missed`. Esta URL deve fazer uso do protocolo HTTPS. | Todos |
| notificationQueryOptions | String | Opcional. Opções de consulta OData para especificar o valor para o recurso de direcionamento. Os clientes recebem notificações quando o recurso atinge ao estado correspondente às opções de consulta aqui fornecidas. Com essa nova propriedade na carga de criação da assinatura, juntamente com todas as propriedades existentes, os Webhooks entregarão notificações sempre que um recurso atingir o estado desejado mencionado na propriedade notificationQueryOptions. Por exemplo, quando o trabalho de impressão é concluído ou quando um valor de propriedade de recurso de trabalho de impressão `isFetchable` torna-se `true` etc. | [Serviço de Impressão Universal](/graph/universal-print-webhook-notifications) |
| notificationUrl | Cadeia de caracteres | Obrigatório. O URL do ponto de extremidade que receberá as notificações de alteração. Este URL deve fazer uso do protocolo HTTPS. | Todos |
| notificationUrlAppId| String | Opcional. A ID do aplicativo que o serviço de assinatura pode usar para gerar o token de validação. Isso permite que o cliente valide a autenticidade da notificação recebida.  | Todos |
| recurso | Cadeia de caracteres | Obrigatório. Especifica o recurso que será monitorado para detectar alterações. Não incluir a URL base (`https://graph.microsoft.com/v1.0/`). Consulte os possíveis valores do [caminho](webhooks.md) do recurso de cada recurso suportado.| Todos |

### <a name="maximum-length-of-subscription-per-resource-type"></a>Tamanho máximo da assinatura por tipo de recurso

| Resource            | Tempo de expiração máximo  |
|:--------------------|:-------------------------|
| **Alerta** de segurança     | 43200 minutos (em 30 dias )  |
| Teams **callRecord**    | 4230 minutos (em 3 dias)  |
| **Canal** do Teams    | 60 minutos (1 hora)  |
| **Chat** do Teams    | 60 minutos (1 hora)  |
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

``` json
{
  "@odata.type": "#microsoft.graph.subscription",
  "id": "String (identifier)",
  "resource": "String",
  "changeType": "String",
  "clientState": "String",
  "notificationUrl": "String",
  "expirationDateTime": "String (timestamp)",
  "applicationId": "String",
  "creatorId": "String",
  "includeResourceData": "Boolean",
  "lifecycleNotificationUrl": "String",
  "encryptionCertificate": "String",
  "encryptionCertificateId": "String",
  "latestSupportedTlsVersion": "String",
  "notificationQueryOptions": "String",
  "notificationUrlAppId": "String"
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
[todoTask]: ./todotask.md

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "subscription resource",
  "keywords": "",
  "section": "documentation",
  "tocPath&quot;: &quot;"
}-->

