---
title: Tipo de recurso serviceUpdateMessage
description: Representa os comunicados de alterações em um serviço.
author: payiAzure
ms.localizationpriority: medium
ms.prod: service-communications
doc_type: resourcePageType
ms.openlocfilehash: e7c8141c5b39d8648c0b3f7bbe37c1af046d9f25
ms.sourcegitcommit: bfd1ab7e015ef04cb2ca3fb85d308ba2ce830a89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/19/2022
ms.locfileid: "62072716"
---
# <a name="serviceupdatemessage-resource-type"></a>Tipo de recurso serviceUpdateMessage

Namespace: microsoft.graph

Representa os comunicados sobre alterações em um serviço.

Representa comunicados como atualizações principais, novos recursos em um produto; por exemplo, a publicação de um novo recurso Windows.

Herda [de serviceAnnouncementBase](../resources/serviceannouncementbase.md).

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter serviceUpdateMessage](../api/serviceupdatemessage-get.md)|[serviceUpdateMessage](../resources/serviceupdatemessage.md)|Recupere as propriedades e as relações de um [objeto serviceUpdateMessage.](../resources/serviceupdatemessage.md) |
|[markRead](../api/serviceupdatemessage-markread.md)|Booliano|Marque uma lista [de serviceUpdateMessage](../resources/serviceupdatemessage.md)s como **lido** para o usuário que está assinado.|
|[markUnread](../api/serviceupdatemessage-markunread.md)|Booliano|Marque uma lista [de serviceUpdateMessage](../resources/serviceupdatemessage.md)s como **não** lido para o usuário insinuável.|
|[archive](../api/serviceupdatemessage-archive.md)|Booliano|Arquivar uma lista [de serviceUpdateMessage](../resources/serviceupdatemessage.md)s para o usuário inscrevedo.|
|[unarchive](../api/serviceupdatemessage-unarchive.md)|Booliano|Unarchive a list of [serviceUpdateMessage](../resources/serviceupdatemessage.md)s for the signed in user.|
|[favorite](../api/serviceupdatemessage-favorite.md)|Booliano|Altere o status de uma lista [de serviceUpdateMessage](../resources/serviceupdatemessage.md)s como favorito para o usuário que está assinado.|
|[unfavorite](../api/serviceupdatemessage-unfavorite.md)|Booliano|Remova o status favorito [de serviceUpdateMessage](../resources/serviceupdatemessage.md)s para o usuário instituto.|
|[Listar anexos](../api/serviceupdatemessage-list-attachments.md)|[Coleção serviceAnnouncementAttachment](../resources/serviceannouncementattachment.md)|Obter uma lista de anexos associados a uma mensagem de serviço.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|actionRequiredByDateTime|DateTimeOffset|O prazo esperado da ação para a mensagem.|
|attachmentsArchive|Stream|O arquivo zip que contém todos os anexos de uma mensagem.|
|corpo|[itemBody](../resources/itembody.md)|O tipo de conteúdo e o conteúdo do corpo da mensagem de serviço.|
|category|serviceUpdateCategory|A categoria de mensagem de serviço. Os valores possíveis são: `preventOrFixIssue`, `planForChange`, `stayInformed`, `unknownFutureValue`.|
|detalhes|Coleção([keyValuePair](../resources/keyvaluepair.md))|Detalhes adicionais sobre a mensagem de serviço. Essa propriedade não dá suporte a filtros. Herdado [do serviceAnnouncementBase](../resources/serviceannouncementbase.md).|
|endDateTime|DateTimeOffset|A hora de término da mensagem de serviço. Herdado [do serviceAnnouncementBase](../resources/serviceannouncementbase.md).|
|hasAttachments|Booliano|Indica se a mensagem tem algum anexo.|
|id|Cadeia de caracteres|A id da mensagem de serviço. Herdado [do serviceAnnouncementBase](../resources/serviceannouncementbase.md).|
|isMajorChange|Booliano|Indica se a mensagem descreve uma atualização importante para o serviço.|
|lastModifiedDateTime|DateTimeOffset|A última hora modificada da mensagem de serviço. Herdado [do serviceAnnouncementBase](../resources/serviceannouncementbase.md).|
|services|Collection(string)|Os serviços afetados pela mensagem de serviço.|
|severity|serviceUpdateSeverity|A gravidade da mensagem de serviço. Os valores possíveis são: `normal`, `high`, `critical`, `unknownFutureValue`.|
|startDateTime|DateTimeOffset|A hora de início da mensagem de serviço. Herdado [do serviceAnnouncementBase](../resources/serviceannouncementbase.md).|
|categorias|Collection(string)|Uma coleção de marcas para a mensagem de serviço. As marcas são fornecidas pela equipe de serviço/equipe de suporte que postam a mensagem para dizer se essa mensagem contém dados de privacidade ou se essa mensagem é para uma nova atualização de recurso de serviço e assim por diante.|
|title|Cadeia de caracteres|O título da mensagem de serviço. Herdado [do serviceAnnouncementBase](../resources/serviceannouncementbase.md).|
|viewPoint|[serviceUpdateMessageViewpoint](../resources/serviceupdatemessageviewpoint.md)|Representa dados de pontos de vista do usuário da mensagem de serviço. Esses dados incluem o status da mensagem, como se o usuário arquivou, leu ou marcou a mensagem como favorita. Essa propriedade é nula quando acessada com permissões de aplicativo.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|attachments|Coleção([serviceAnnouncementAttachment](../resources/serviceannouncementattachment.md))|Uma coleção [de serviceAnnouncementAttachments](../resources/serviceannouncementattachment.md).|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.serviceUpdateMessage",
  "baseType": "microsoft.graph.serviceAnnouncementBase",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.serviceUpdateMessage",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "title": "String",
  "details": [
    {
      "@odata.type": "microsoft.graph.keyValuePair"
    }
  ],
  "id": "String (identifier)",
  "body": {
    "@odata.type": "microsoft.graph.itemBody"
  },
  "category": "String",
  "severity": "String",
  "tags": [
    "String"
  ],
  "isMajorChange": "Boolean",
  "actionRequiredByDateTime": "String (timestamp)",
  "services": [
    "String"
  ],
  "viewPoint": {
    "@odata.type": "microsoft.graph.serviceUpdateMessageViewpoint"
  },
  "hasAttachments": "Boolean",
  "attachmentsArchive": "Stream"
}
```

