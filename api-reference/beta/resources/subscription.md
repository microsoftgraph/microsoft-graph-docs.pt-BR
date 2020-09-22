---
title: tipo de recurso de assinatura
description: 'Uma assinatura que permite a um aplicativo cliente receber notificações sobre alterações de dados no Microsoft Graph. Atualmente, as assinaturas estão habilitadas para as seguintes coleções de recursos:'
localization_priority: Normal
author: davidmu1
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 95312f2e95899ec160d9217cf896052b6463d393
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48058022"
---
# <a name="subscription-resource-type"></a>tipo de recurso de assinatura

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma assinatura que permite a um aplicativo cliente receber notificações sobre alterações de dados no Microsoft Graph. Atualmente, as assinaturas estão habilitadas para as seguintes coleções de recursos:

- Um [alerta][] do Microsoft Graph Security API
- Uma [callRecord][] produzida após uma chamada ou uma reunião no Microsoft Teams
- Um [chat][] enviado por meio de equipes ou canais no Microsoft Teams
- Uma [conversa][] em um grupo no Microsoft 365
- Conteúdo da hierarquia de uma pasta raiz [driveItem][] no OneDrive for Business ou de uma pasta raiz ou uma subpasta [driveItem][] no OneDrive pessoal do usuário
- Uma [lista][] em um [site][] do SharePoint
- Uma [mensagem][], [evento][] ou [contato][] no Outlook
- A [presença][] de um usuário no Microsoft Teams
- Um [usuário][] ou [grupo][] no Azure Active Directory

Consulte [usar o Microsoft Graph API para obter notificações de alteração](webhooks.md) dos possíveis valores de caminho de recurso de cada recurso suportado.

## <a name="methods"></a>Métodos

| Método | Tipo de retorno | Descrição |
|:-------|:------------|:------------|
| [Criar assinatura](../api/subscription-post-subscriptions.md) | [assinatura](subscription.md) | Assina um aplicativo de escuta para receber notificações sobre alterações nos dados do Microsoft Graph. |
| [Atualizar assinatura](../api/subscription-update.md) | [subscription](subscription.md) | Renovar uma assinatura atualizando seu tempo de expiração. |
| [Listar de assinaturas](../api/subscription-list.md) | [assinatura](subscription.md) | Lista assinaturas ativas. |
| [Obter assinatura](../api/subscription-get.md) | [subscription](subscription.md) | Leia as propriedades e as relações do objeto Subscription. |
| [Excluir assinatura](../api/subscription-delete.md) | Nenhuma | Excluir um objeto Subscription. |

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------|:-----|:------------|
| changeType | cadeia de caracteres | Indica qual é o tipo de alteração no recurso inscrito que irá emitir uma notificação de alteração. Os valores com suporte são: `created`, `updated`, `deleted`. Vários valores podem ser combinados usando uma lista separada por vírgula. Obrigatório. <br><br>Observação: As notificações de alteração de lista e item raiz da unidade suportam apenas o `updated` changeType. Suporte para notificações de alteração de usuário e grupo `updated` e `deleted` changeType. |
| notificationUrl | cadeia de caracteres | A URL do ponto de extremidade que recebe as notificações de alteração. Esta URL deve usar o protocolo HTTPS. Obrigatório. |
| lifecycleNotificationUrl | cadeia de caracteres | A URL do ponto de extremidade que recebe notificações de ciclo de vida, incluindo `subscriptionRemoved` e `missed` notificações. Se não for fornecido, as notificações serão entregues ao **notificationUrl**. Esta URL deve usar o protocolo HTTPS. Opcional. <br><br>[Leia mais](/graph/webhooks-outlook-authz) sobre como os recursos do Outlook usam notificações de ciclo de vida. |
| recurso | cadeia de caracteres | Especifica o recurso que será monitorado para detectar alterações. Não incluir a URL base (`https://graph.microsoft.com/beta/`). Consulte os possíveis valores do [caminho](webhooks.md) do recurso de cada recurso suportado. Obrigatório. |
| expirationDateTime | DateTimeOffset | Especifica a data e a hora em que a assinatura do webhook expira. O horário está em UTC e pode ser uma quantidade de tempo desde a criação da assinatura que varia para o recurso assinado.  Confira na tabela abaixo o tempo máximo permitido para a assinatura. Obrigatório. |
| clientState | string | Especifica o valor da propriedade **ClientState** enviada pelo serviço em cada notificação de alteração. O tamanho máximo é de 255 caracteres. O cliente pode verificar se a notificação de alteração veio do serviço, comparando o valor da propriedade **ClientState** enviada com a assinatura com o valor da propriedade **ClientState** recebida com cada notificação de alteração. Opcional. |
| id | string | Identificador exclusivo da assinatura. Somente leitura. |
| ApplicationId | cadeia de caracteres | Identificador do aplicativo usado para criar a assinatura. Somente leitura. |
| creatorId | cadeia de caracteres | Identificador de usuário ou entidade de serviço que criou a assinatura. Se o aplicativo usou permissões delegadas para criar a assinatura, este campo conterá a ID do usuário conectado o aplicativo chamado em nome de. Se o aplicativo usava permissões de aplicativo, este campo contém a ID da entidade de serviço correspondente ao aplicativo. Somente leitura. |
| includeResourceData | Booliano | Quando definido como `true` , as notificações de alteração [incluem dados de recurso](/graph/webhooks-with-resource-data) (como o conteúdo de uma mensagem de chat). Opcional. | 
| encryptionCertificate | cadeia de caracteres | Uma representação codificada em Base64 de um certificado com uma chave pública usada para criptografar dados de recurso em notificações de alteração. Opcional. Obrigatório quando **includeResourceData** é true. | 
| encryptionCertificateId | cadeia de caracteres | Um identificador personalizado fornecido pelo aplicativo para ajudar a identificar o certificado necessário para descriptografar dados de recurso. Opcional. Obrigatório quando **includeResourceData** é true. |
| latestSupportedTlsVersion | Cadeia de caracteres | Especifica a versão mais recente do protocolo TLS que o ponto de extremidade, especificado por **notificationUrl**, é compatível. Os valores possíveis são: `v1_0`, `v1_1`, `v1_2`, `v1_3`. </br></br>Para os assinantes cujo ponto de extremidade de notificação suporta uma versão menor que a versão recomendada atualmente (TLS 1.2), especificar essa propriedade por uma [linha do tempo](https://developer.microsoft.com/graph/blogs/microsoft-graph-subscriptions-deprecating-tls-1-0-and-1-1/) definida, permite o uso temporário da versão preterida do TLS antes de concluir a atualização para o TLS 1.2. Para esses assinantes, não definir essa propriedade pela linha do tempo resultaria em uma falha nas operações da assinatura. </br></br>Para os assinantes cujo ponto de extremidade já tem suporte ao TLS 1.2, a configuração dessa propriedade é opcional. Nesses casos, o Microsoft Graph padroniza a propriedade como `v1_2`. |

### <a name="maximum-length-of-subscription-per-resource-type"></a>Tamanho máximo da assinatura por tipo de recurso

| Resource            | Tempo de expiração máximo  |
|:--------------------|:-------------------------|
| **Alerta** de segurança     | 43200 minutos (em 30 dias )  |
| **callRecord** do Teams    | 4230 minutos (em 3 dias)  |
| Teams **chat**    | 60 minutos (1 hora)  |
| **Conversa** de grupo | 4230 minutos (em 3 dias)    |
| OneDrive **driveItem**    | 4230 minutos (em 3 dias)    |
| **Lista** do SharePoint    | 4230 minutos (em 3 dias)    |
| **Mensagem**, **evento**, **contato** do Outlook              | 4230 minutos (em 3 dias)    |
| **usuário**, **grupo**, outros recursos de diretório   | 4230 minutos (em 3 dias)    |
| **presence**        | 60 minutos (1 hora) |


> **Observação:** Os aplicativos existentes e os novos aplicativos não devem ultrapassar o valor suportado. No futuro, as solicitações para criar ou renovar uma assinatura além do valor máximo falharão.

## <a name="relationships"></a>Relações

Nenhum

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
  "creatorId": "string",
  "includeResourceData": "boolean",
  "encryptionCertificate": "string",
  "encryptionCertificateId": "string",
  "latestSupportedTlsVersion": "string"
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


