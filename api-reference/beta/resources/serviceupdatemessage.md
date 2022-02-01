---
title: Tipo de recurso serviceUpdateMessage
description: Representa os comunicados de alterações em um serviço.
author: payiAzure
ms.localizationpriority: medium
ms.prod: service-communications
doc_type: resourcePageType
ms.openlocfilehash: 2c9cf7fbf4551fa8fe47b14a93b49389b710c747
ms.sourcegitcommit: 15956da1b4a7d523363ffa8afb5e2059fbf680ce
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/01/2022
ms.locfileid: "62290466"
---
# <a name="serviceupdatemessage-resource-type"></a>Tipo de recurso serviceUpdateMessage

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os comunicados sobre alterações em um serviço.

Representa comunicados como atualizações principais, novos recursos em um produto; por exemplo, a publicação de um novo recurso SharePoint.

Herda [de serviceAnnouncementBase](../resources/serviceannouncementbase.md).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter serviceUpdateMessage](../api/serviceupdatemessage-get.md)|[serviceUpdateMessage](../resources/serviceupdatemessage.md)|Recupere as propriedades e as relações de um [objeto serviceUpdateMessage](../resources/serviceupdatemessage.md) . |
|[markRead](../api/serviceupdatemessage-markread.md)|Boolean|Marque uma lista [de serviceUpdateMessages](../resources/serviceupdatemessage.md) como **lido** para o usuário que está assinado.|
|[markUnread](../api/serviceupdatemessage-markunread.md)|Booliano|Marque uma lista [de serviceUpdateMessages](../resources/serviceupdatemessage.md) como **não** lido para o usuário que está assinado.|
|[archive](../api/serviceupdatemessage-archive.md)|Booliano|Arquivar uma lista [de serviceUpdateMessages](../resources/serviceupdatemessage.md) para o usuário inscrevedo.|
|[unarchive](../api/serviceupdatemessage-unarchive.md)|Booliano|Unarchive a list of [serviceUpdateMessages](../resources/serviceupdatemessage.md) for the signed in user.|
|[favorite](../api/serviceupdatemessage-favorite.md)|Booliano|Altere o status de uma lista [de serviceUpdateMessages](../resources/serviceupdatemessage.md) como favorito para o usuário que está assinado.|
|[unfavorite](../api/serviceupdatemessage-unfavorite.md)|Booliano|Remova o status favorito [do serviceUpdateMessages](../resources/serviceupdatemessage.md) para o usuário que está assinado.|
|[Listar anexos](../api/serviceupdatemessage-list-attachments.md)|[Coleção serviceAnnouncementAttachment](../resources/serviceannouncementattachment.md)|Obter uma lista de anexos associados a uma mensagem de serviço.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|actionRequiredByDateTime|DateTimeOffset|O prazo esperado da ação para a mensagem.|
|attachmentsArchive|Stream|O arquivo zip de todos os anexos de uma mensagem.|
|corpo|[itemBody](../resources/itembody.md)|O tipo de conteúdo e o conteúdo do corpo da mensagem de serviço.|
|category|serviceUpdateCategory|A categoria de mensagem de serviço. Os valores possíveis são: `preventOrFixIssue`, `planForChange`, `stayInformed`, `unknownFutureValue`.|
|detalhes|Collection([keyValuePair](../resources/keyvaluepair.md))|Detalhes adicionais sobre a mensagem de serviço. Essa propriedade não dá suporte a filtros. Herdado [do serviceAnnouncementBase](../resources/serviceannouncementbase.md).|
|endDateTime|DateTimeOffset|A hora de término da mensagem de serviço. Herdado [do serviceAnnouncementBase](../resources/serviceannouncementbase.md).|
|hasAttachments|Booliano|Indica se a mensagem tem algum anexo.|
|id|Cadeia de caracteres|A id da mensagem de serviço. Herdado [do serviceAnnouncementBase](../resources/serviceannouncementbase.md).|
|isMajorChange|Boolean|Indica se a mensagem descreve uma atualização importante para o serviço.|
|lastModifiedDateTime|DateTimeOffset|A última hora modificada da mensagem de serviço. Herdado [do serviceAnnouncementBase](../resources/serviceannouncementbase.md).|
|services|Collection(string)|Os serviços afetados pela mensagem de serviço.|
|severity|serviceUpdateSeverity|A gravidade da mensagem de serviço. Os valores possíveis são: `normal`, `high`, `critical`, `unknownFutureValue`.|
|startDateTime|DateTimeOffset|A hora de início da mensagem de serviço. Herdado [do serviceAnnouncementBase](../resources/serviceannouncementbase.md).|
|categorias|Collection(string)|Uma coleção de marcas para a mensagem de serviço. As marcas são fornecidas pela equipe de serviço/equipe de suporte que postam a mensagem para dizer se essa mensagem contém dados de privacidade ou se essa mensagem é para uma nova atualização de recurso de serviço e assim por diante.|
|title|String|O título da mensagem de serviço. Herdado [do serviceAnnouncementBase](../resources/serviceannouncementbase.md).|
|viewPoint|[serviceUpdateMessageViewpoint](../resources/serviceupdatemessageviewpoint.md)|Representa dados de pontos de vista do usuário da mensagem de serviço. Esses dados incluem o status da mensagem, como se o usuário arquivou, leu ou marcou a mensagem como favorita. Essa propriedade é nula quando acessada com permissões de aplicativo.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|attachments|Collection([serviceAnnouncementAttachment](../resources/serviceannouncementattachment.md))|Uma coleção [de serviceAnnouncementAttachments](../resources/serviceannouncementattachment.md).|

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

