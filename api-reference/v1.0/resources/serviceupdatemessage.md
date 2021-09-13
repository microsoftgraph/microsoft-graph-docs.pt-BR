---
title: Tipo de recurso serviceUpdateMessage
description: Representa os comunicados de alterações em um serviço.
author: payiAzure
ms.localizationpriority: medium
ms.prod: service-communications
doc_type: resourcePageType
ms.openlocfilehash: 7e8dc6e63025400c64114dc282389fc2f7453daf
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59108818"
---
# <a name="serviceupdatemessage-resource-type"></a>Tipo de recurso serviceUpdateMessage

Namespace: microsoft.graph

Representa os comunicados sobre alterações em um serviço.

Representa comunicados como atualizações principais, novos recursos em um produto; por exemplo, a publicação de um novo recurso Windows.

Herda [de serviceAnnouncementBase](../resources/serviceannouncementbase.md).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter serviceUpdateMessage](../api/serviceupdatemessage-get.md)|[serviceUpdateMessage](../resources/serviceupdatemessage.md)|Recupere as propriedades e as relações de um [objeto serviceUpdateMessage.](../resources/serviceupdatemessage.md) |
|[markRead](../api/serviceupdatemessage-markread.md)|Booliano|Marque uma lista [de serviceUpdateMessage](../resources/serviceupdatemessage.md)s como **lido** para o usuário que está assinado.|
|[markUnread](../api/serviceupdatemessage-markunread.md)|Booliano|Marque uma lista [de serviceUpdateMessage](../resources/serviceupdatemessage.md)s como **não** lido para o usuário insinuável.|
|[archive](../api/serviceupdatemessage-archive.md)|Booliano|Arquivar uma lista [de serviceUpdateMessage](../resources/serviceupdatemessage.md)s para o usuário inscrevedo.|
|[unarchive](../api/serviceupdatemessage-unarchive.md)|Booliano|Unarchive a list of [serviceUpdateMessage](../resources/serviceupdatemessage.md)s for the signed in user.|
|[favorite](../api/serviceupdatemessage-favorite.md)|Booliano|Altere o status de uma lista [de serviceUpdateMessage](../resources/serviceupdatemessage.md)s como favorito para o usuário que está assinado.|
|[unfavorite](../api/serviceupdatemessage-unfavorite.md)|Booliano|Remova o status favorito [de serviceUpdateMessage](../resources/serviceupdatemessage.md)s para o usuário instituto.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|actionRequiredByDateTime|DateTimeOffset|O prazo esperado da ação para a mensagem.|
|corpo|[itemBody](../resources/itembody.md)|O tipo de conteúdo e o conteúdo do corpo da mensagem de serviço.|
|category|serviceUpdateCategory|A categoria de mensagem de serviço. Os valores possíveis são: `preventOrFixIssue`, `planForChange`, `stayInformed`, `unknownFutureValue`.|
|detalhes|Coleção([keyValuePair](../resources/keyvaluepair.md))|Detalhes adicionais sobre a mensagem de serviço. Essa propriedade não dá suporte a filtros. Herdado [do serviceAnnouncementBase](../resources/serviceannouncementbase.md).|
|endDateTime|DateTimeOffset|A hora de término da mensagem de serviço. Herdado [do serviceAnnouncementBase](../resources/serviceannouncementbase.md).|
|id|Cadeia de caracteres|A id da mensagem de serviço. Herdado [do serviceAnnouncementBase](../resources/serviceannouncementbase.md).|
|isMajorChange|Boolean|Indica se a mensagem descreve uma atualização importante para o serviço.|
|lastModifiedDateTime|DateTimeOffset|A última hora modificada da mensagem de serviço. Herdado [do serviceAnnouncementBase](../resources/serviceannouncementbase.md).|
|services|Collection(string)|Os serviços afetados pela mensagem de serviço.|
|severity|serviceUpdateSeverity|A gravidade da mensagem de serviço. Os valores possíveis são: `normal`, `high`, `critical`, `unknownFutureValue`.|
|startDateTime|DateTimeOffset|A hora de início da mensagem de serviço. Herdado [do serviceAnnouncementBase](../resources/serviceannouncementbase.md).|
|categorias|Collection(string)|Uma coleção de marcas para a mensagem de serviço.|
|title|String|O título da mensagem de serviço. Herdado [do serviceAnnouncementBase](../resources/serviceannouncementbase.md).|
|viewPoint|[serviceUpdateMessageViewpoint](../resources/serviceupdatemessageviewpoint.md)|Representa os dados de pontos de exibição do usuário da mensagem de serviço. Esses dados incluem o status da mensagem, como se o usuário arquivou, leu ou marcou a mensagem como favorita. Essa propriedade é nula quando acessada com permissões de aplicativo.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.serviceUpdateMessage",
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
  }
}
```

