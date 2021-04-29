---
title: Tipo de recurso dataSourceContainer
description: Classe base para custodiantes e fontes de dados não custodiais.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: e2d7d88a3d747817858853ebc6f2909b2edde65b
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/29/2021
ms.locfileid: "52080719"
---
# <a name="datasourcecontainer-resource-type"></a>Tipo de recurso dataSourceContainer

Namespace: microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Classe base [para custodiante](../resources/ediscovery-custodian.md) [e nãocustodialDataSource](../resources/ediscovery-noncustodialdatasource.md).

Herda da [entidade](../resources/entity.md).

## <a name="methods"></a>Métodos

Nenhum

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|Data e hora criadas da entidade dataSourceContainer.|
|displayName|String|Nome de exibição da entidade dataSourceContainer.|
|id|String|Identificador exclusivo do dataSourceContainer. Herdado da [entidade](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|Data e hora da última modificação do dataSourceContainer.|
|releasedDateTime|DateTimeOffset|Data e hora em que o dataSourceContainer foi liberado do caso.|
|status|microsoft.graph.ediscovery.dataSourceContainerStatus|Status mais recente do dataSourceContainer. Os valores possíveis são: `Active` e `Released`.|

### <a name="datasourcecontainerstatus-values"></a>valores dataSourceContainerStatus

|Member|Descrição|
|:---|:---|
|Ativo|O dataSourceContainer está em espera no caso.|
|Lançado|O dataSourceContainer foi liberado de espera no caso.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.dataSourceContainer",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.dataSourceContainer",
  "id": "String (identifier)",
  "status": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "releasedDateTime": "String (timestamp)",
  "displayName": "String",
  "createdDateTime": "String (timestamp)"
}
```
