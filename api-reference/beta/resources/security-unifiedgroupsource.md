---
title: Tipo de recurso unifiedGroupSource
description: O contêiner do grupo de um guardião.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 3e544a4b6d00bb59b5879fc13376fd94a5bba169
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/08/2022
ms.locfileid: "65945021"
---
# <a name="unifiedgroupsource-resource-type"></a>Tipo de recurso unifiedGroupSource

Namespace: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O contêiner do grupo de um guardião.

Herda de [dataSource](../resources/security-datasource.md).

## <a name="methods"></a>Métodos
Nenhum.
## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|createdBy|[identitySet](../resources/identityset.md)|O usuário que criou **o unifiedGroupSource**.|
|createdDateTime|DateTimeOffset|A data e a hora em que **o unifiedGroupSource** foi criado.|
|displayName|String|O nome de exibição do grupo unificado - Esse é o nome do grupo.|
|id|String|A ID do **unifiedGroupSource**. Essa não é a ID do grupo real.|
|includedSources|Cadeia de caracteres|Especifica quais fontes estão incluídas neste grupo. Os valores possíveis são: `mailbox` e `site`.|
|holdStatus|Cadeia de caracteres|O status de retenção do **unifiedGroupSource**. Os valores possíveis são: `notApplied`, `applied`, `applying`, , `removing``partial`|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|group|[Grupo](../resources/group.md)|Representar um grupo.|

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

