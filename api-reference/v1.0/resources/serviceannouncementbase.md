---
title: Tipo de recurso serviceAnnouncementBase
description: Esse é um tipo de base abstrato para serviceHealthIssue e serviceUpdateMessage.
author: payiAzure
ms.localizationpriority: medium
ms.prod: service-communications
doc_type: resourcePageType
ms.openlocfilehash: 8ea4ddaed2a3ea67833be103da58f703957f2373
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59019136"
---
# <a name="serviceannouncementbase-resource-type"></a>Tipo de recurso serviceAnnouncementBase

Namespace: microsoft.graph

Este é um tipo de base abstrato [para serviceHealthIssue](../resources/servicehealthissue.md) e [serviceUpdateMessage](../resources/serviceupdatemessage.md).

Herda da [entidade](../resources/entity.md).

## <a name="methods"></a>Métodos
Nenhum.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|detalhes|Coleção([keyValuePair](../resources/keyvaluepair.md))|Detalhes adicionais sobre o evento de serviço. Essa propriedade não dá suporte a filtros.|
|endDateTime|DateTimeOffset|A hora de término do evento de serviço.|
|id|Cadeia de caracteres|A id do evento de serviço.|
|lastModifiedDateTime|DateTimeOffset|A última hora modificada do evento de serviço.|
|startDateTime|DateTimeOffset|A hora de início do evento de serviço.|
|title|String|O título do evento de serviço.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.serviceAnnouncementBase",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.serviceAnnouncementBase",
  "id": "String (identifier)",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "title": "String",
  "details": [
    {
      "@odata.type": "microsoft.graph.keyValuePair"
    }
  ]
}
```
