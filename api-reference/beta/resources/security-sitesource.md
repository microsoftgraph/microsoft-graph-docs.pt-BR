---
title: Tipo de recurso siteSource
description: O contêiner de um site associado a um guardião.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 0dd23c703ef63c11da357ac6db0d0dfdc73a5212
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/18/2022
ms.locfileid: "66837531"
---
# <a name="sitesource-resource-type"></a>Tipo de recurso siteSource

Namespace: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
O contêiner de um site associado a um guardião.

Herda de [dataSource](../resources/security-datasource.md).


## <a name="methods"></a>Métodos
Nenhum.
## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|createdBy|[identitySet](../resources/identityset.md)|O usuário que criou **o siteSource**.|
|createdDateTime|DateTimeOffset|A data e a hora em **que o siteSource** foi criado.|
|displayName|Cadeia de caracteres|O nome de exibição **do siteSource**. Esse será o nome do site do SharePoint.|
|id|String| A ID do **siteSource**. |
|holdStatus|microsoft.graph.security.dataSourceHoldStatus|O status de retenção do **siteSource**. Os valores possíveis são: `notApplied`, `applied`, `applying`, `removing`, `partial`.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|site|[site](../resources/site.md)|O site do SharePoint associado ao **siteSource**.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.siteSource",
  "baseType": "microsoft.graph.security.dataSource",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.siteSource",
  "id": "String (identifier)",
  "displayName": "String",
  "holdStatus": "String",
  "createdDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```

