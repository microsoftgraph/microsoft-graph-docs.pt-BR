---
title: Tipo de recurso serviceAnnouncementBase
description: Esse é um tipo de base abstrato para serviceHealthIssue e serviceUpdateMessage.
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: resourcePageType
ms.openlocfilehash: 5e1c8783615645461d3dc7bafdb403e52c94cf4bebd3f7e8cc5d6bbd3d1aec0a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54195581"
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
|id|String|A id do evento de serviço.|
|lastModifiedDateTime|DateTimeOffset|A última hora modificada do evento de serviço.|
|startDateTime|DateTimeOffset|A hora de início do evento de serviço.|
|title|Cadeia de caracteres|O título do evento de serviço.|

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