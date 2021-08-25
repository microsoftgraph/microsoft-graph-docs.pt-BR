---
title: tipo de recurso post
description: Representa um item Post individual em uma entidade conversationThread.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: f1af505f7c55ef46c855d92170679195bb390474
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/25/2021
ms.locfileid: "58513192"
---
# <a name="post-resource-type"></a>tipo de recurso post

Namespace: microsoft.graph Representa um item Post individual dentro de uma [entidade conversationThread.](conversationthread.md)

Embora você não possa criar explicitamente uma postagem, seguir um destes procedimentos criaria uma postagem:

- [Responder a uma postagem existente](../api/post-reply.md) 
- [Responder a um thread existente](../api/conversationthread-reply.md) 
- [Criar um thread em uma nova conversa](../api/group-post-threads.md)
- [Criar uma nova conversa](../api/group-post-conversations.md)

Esse recurso permite que você adicione seus próprios dados às propriedades personalizadas usando [extensions](/graph/extensibility-overview).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Listar postagens](../api/conversationthread-list-posts.md) | [post](post.md) |Obtenha as postagens do thread especificado. |
|[Obter postagem](../api/post-get.md) | [post](post.md) |Obtenha as propriedades e os relacionamentos de uma postagem em um thread especificado.|
|[Responder](../api/post-reply.md)|Nenhuma|Responda a uma postagem e adicione uma nova postagem ao thread especificado em uma conversa de grupo.|
|[Encaminhar](../api/post-forward.md)|Nenhuma|Encaminhe uma postagem para um destinatário.|
|**Anexos**| | |
|[List attachments](../api/post-list-attachments.md) |Coleção [attachment](attachment.md)| Obtenha todos os anexos em uma postagem.|
|[Add attachment](../api/post-post-attachments.md) |[attachment](attachment.md)| Adicione um anexo a uma postagem. |
|**Extensões abertas**| | |
|[Criar extensão aberta](../api/opentypeextension-post-opentypeextension.md) |[openTypeExtension](opentypeextension.md)| Criar uma extensão aberta e adicionar propriedades personalizadas em uma instância nova ou existente de um recurso.|
|[Obter extensão aberta](../api/opentypeextension-get.md) |Coleção [openTypeExtension](opentypeextension.md)| Obter um ou mais objetos de extensão ou identificados por nome ou nome totalmente qualificado.|
|**Extensões de esquema**| | |
|[Adicionar valores de extensões de esquema](/graph/extensibility-schema-groups) || Cria uma definição para a extensão de esquema e usa-a para adicionar dados digitados personalizados a um recurso.|
|**Propriedades estendidas**| | |
|[Criar uma propriedade estendida de valor único](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[post](post.md)  |Criar uma ou mais propriedades estendidas de valor único em uma postagem nova ou existente.   |
|[Obter postagem com propriedade estendida de valor único](../api/singlevaluelegacyextendedproperty-get.md)  | [post](post.md) | Obtenha postagens que contenham uma propriedade estendida de valor único usando `$expand` ou `$filter`. |
|[Criar propriedade estendida de vários valores](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [post](post.md) | Crie uma ou mais propriedades estendidas de vários valores em uma postagem nova ou existente.  |
|[Obter postagem com propriedade estendida de vários valores](../api/multivaluelegacyextendedproperty-get.md)  | [post](post.md) | Obtenha uma postagem que contenha uma propriedade estendida de vários valores usando `$expand`. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|body|[itemBody](itembody.md)|O conteúdo da postagem. Esta é uma propriedade padrão. Esta propriedade pode ser nula.|
|categories|String collection|As categorias associadas à postagem.|
|changeKey|String|Identifica a versão da postagem. Toda vez que a postagem muda, ChangeKey também muda. Isso permite que o Exchange aplique alterações na versão correta do objeto.|
|conversationId|String|ID exclusiva da conversa. Somente leitura.|
|conversationThreadId|String|ID exclusiva do thread de conversa. Somente leitura.|
|createdDateTime|DateTimeOffset|Especifica quando a postagem foi criada. O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|from|[recipient](recipient.md)|Usado em cenários de acesso de representante. Indica quem postou a mensagem em nome de outro usuário. Esta é uma propriedade padrão.|
|hasAttachments|Booliano|Indica se a postagem tem pelo menos um anexo. Esta é uma propriedade padrão.|
|id|String| Somente leitura.|
|lastModifiedDateTime|DateTimeOffset|Especifica quando a postagem foi modificada pela última vez. O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|newParticipants|Coleção [recipient](recipient.md)|Participantes da conversa que foram adicionados ao thread como parte desta postagem.|
|receivedDateTime|DateTimeOffset|Especifica quando a postagem foi recebida. O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|sender|[recipient](recipient.md)|Contém o endereço do remetente. O valor de Sender será considerado o endereço do usuário autenticado caso o remetente não seja especificado. Esta é uma propriedade padrão.|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|attachments|Coleção [Attachment](attachment.md)| Somente leitura. Anulável. Suporta o `$expand`.|
|extensions|Coleção [Extension](extension.md)|A coleção de extensões abertas definidas para a postagem. Somente leitura. Anulável. Suporta o `$expand`.|
|inReplyTo|[post](post.md)| Somente leitura. Oferece suporte para `$expand`.|
|multiValueExtendedProperties|Coleção [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)| A coleção de propriedades estendidas de vários valores definidas para a postagem. Somente leitura. Anulável.|
|singleValueExtendedProperties|Coleção [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)| A coleção de propriedades estendidas de valor único definidas para a postagem. Somente leitura. Anulável.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [
    "attachments",
    "inReplyTo",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "baseType": "microsoft.graph.outlookItem",
  "@odata.type": "microsoft.graph.post",
  "@odata.annotations": [
    {
      "property": "attachments",
      "capabilities": {
        "changeTracking": false,
        "searchable": false,
        "updatable": false
      }
    },
    {
      "property": "extensions",
      "capabilities": {
        "changeTracking": false,
        "searchable": false
      }
    },
    {
      "property": "inReplyTo",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "insertable": false,
        "navigability": "single",
        "searchable": false,
        "updatable": false
      }
    }
  ]
}-->

```json
{
  "body": {"@odata.type": "microsoft.graph.itemBody"},
  "categories": ["string"],
  "changeKey": "string",
  "conversationId": "string",
  "conversationThreadId": "string",
  "createdDateTime": "String (timestamp)",
  "from": {"@odata.type": "microsoft.graph.recipient"},
  "hasAttachments": true,
  "id": "string (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "newParticipants": [{"@odata.type": "microsoft.graph.recipient"}],
  "receivedDateTime": "String (timestamp)",
  "sender": {"@odata.type": "microsoft.graph.recipient"}
}

```

## <a name="see-also"></a>Confira também

- [Adicionar dados personalizados a recursos usando extensões](/graph/extensibility-overview)
- [Adicionar dados personalizados aos usuários usando extensões abertas](/graph/extensibility-open-users)
- [Adicionar dados personalizados a grupos usando as extensões do esquema](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "post resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

