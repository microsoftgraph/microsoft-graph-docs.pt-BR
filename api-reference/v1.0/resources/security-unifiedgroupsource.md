---
title: Tipo de recurso unifiedGroupSource
description: O contêiner do grupo de um guardião.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: d17db0d4051a480806fb0d1aafdcb08ff24b0ca6
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/18/2022
ms.locfileid: "66839043"
---
# <a name="unifiedgroupsource-resource-type"></a>Tipo de recurso unifiedGroupSource

Namespace: microsoft.graph.security



O contêiner do grupo de um guardião.

Herda de [dataSource](../resources/security-datasource.md).

## <a name="methods"></a>Métodos
Nenhum.
## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|createdBy|[identitySet](../resources/identityset.md)|O usuário que criou **o unifiedGroupSource**.|
|createdDateTime|DateTimeOffset|A data e a hora em que **o unifiedGroupSource** foi criado.|
|displayName|Cadeia de caracteres|O nome de exibição do grupo unificado, que é o nome do grupo.|
|id|String|A ID do **unifiedGroupSource**. Essa não é a ID do grupo real.|
|includedSources|microsoft.graph.security.sourceType|Especifica quais fontes estão incluídas neste grupo. Os valores possíveis são: `mailbox` e `site`.|
|holdStatus|microsoft.graph.security.dataSourceHoldStatus|O status de retenção do **unifiedGroupSource**. Os valores possíveis são: `notApplied`, `applied`, `applying`, , `removing``partial`|

### <a name="sourcetype-values"></a>Valores sourceType
|Member|Descrição|
|:----|-----------|
| mailbox | Representa uma caixa de correio.|
| site | Representa um site do SharePoint.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|group|[grupo](../resources/group.md)|Representa um grupo.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.unifiedGroupSource",
  "baseType": "microsoft.graph.security.dataSource",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.unifiedGroupSource",
  "id": "String (identifier)",
  "displayName": "String",
  "holdStatus": "String",
  "createdDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "includedSources": "String"
}
```

