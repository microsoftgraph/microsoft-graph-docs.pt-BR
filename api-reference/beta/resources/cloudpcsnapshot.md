---
title: Tipo de recurso cloudPcSnapshot
description: Representa um instantâneo de computador na nuvem.
author: xintaozMS
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 14cf7ecffe7980db32abf81d475f45ac5725c64c
ms.sourcegitcommit: b19b19bf192688f4c513492e8391e4d8dc104633
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/17/2022
ms.locfileid: "62878765"
---
# <a name="cloudpcsnapshot-resource-type"></a>Tipo de recurso cloudPcSnapshot

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um instantâneo das configurações de dispositivo de um computador na nuvem que pode ser usado para restaurar o sistema de dispositivos.


Herda da [entidade](../resources/entity.md).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar instantâneos](../api/virtualendpoint-list-snapshots.md)|[Coleção cloudPcSnapshot](../resources/cloudpcsnapshot.md)|Obter uma lista dos [objetos cloudPcSnapshot](../resources/cloudpcsnapshot.md) e suas propriedades.|
|[Obter cloudPcSnapshot](../api/cloudpcsnapshot-get.md)|[cloudPcSnapshot](../resources/cloudpcsnapshot.md)|Leia as propriedades e as relações de um [objeto cloudPcSnapshot](../resources/cloudpcsnapshot.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|cloudPcId|Cadeia de caracteres|O identificador exclusivo para o Cloud PC.|
|createdDateTime|DateTimeOffset|A data e a hora em que o instantâneo foi tirado. O timestamp é mostrado no formato ISO 8601 e tempo universal coordenado (UTC). Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.|
|id|String|O identificador exclusivo para o instantâneo do dispositivo cloud pc em um ponto específico no tempo. Herdado da [entidade](../resources/entity.md).|
|lastRestoredDateTime|DateTimeOffset|A data e a hora em que o instantâneo foi usado pela última vez para restaurar o dispositivo cloud pc. O timestamp é mostrado no formato ISO 8601 e tempo universal coordenado (UTC). Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.|
|status|[cloudPcSnapshotStatus](#cloudpcsnapshotstatus-values)|O status do instantâneo do computador na nuvem. Os valores possíveis são: `ready`, `unknownFutureValue`.|

### <a name="cloudpcsnapshotstatus-values"></a>valores cloudPcSnapshotStatus 

|Member|Descrição|
|:---|:---|
|ready|O instantâneo está pronto para restaurar o dispositivo cloud pc.|
|unknownFutureValue|Valor de sentinela de enumeração evolvável. Não usar.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.cloudPcSnapshot",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.cloudPcSnapshot",
  "cloudPcId": "String",
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "lastRestoredDateTime": "String (timestamp)",
  "status": "String"
}
```

