---
title: Tipo de recurso dataSourceContainer
description: Classe base para fontes de dados custodiantes e não custodiais.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 7482e31ab1a43cf4c60e7c211acb38d8cac42bfa
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/08/2022
ms.locfileid: "65945059"
---
# <a name="datasourcecontainer-resource-type"></a>Tipo de recurso dataSourceContainer

Namespace: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Classe base [para eDiscoveryCustodian](../resources/security-ediscoverycustodian.md) [e eDiscoveryNonCutodialDataSource](../resources/security-ediscoverynoncustodialdatasource.md) Este é um tipo abstrato.
Herda de [entidade](../resources/entity.md).

## <a name="methods"></a>Métodos

Nenhum.
## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|holdStatus|String|O status de retenção do dataSourceContainer.Os valores possíveis são: `notApplied`, `applied`, `applying`, , `removing``partial`|
|createdDateTime|DateTimeOffset|Data e hora criadas da entidade dataSourceContainer.|
|displayName|Cadeia de caracteres|Nome de exibição da entidade dataSourceContainer.|
|id|Cadeia de caracteres|Identificador exclusivo do dataSourceContainer. Herdado da [entidade](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|Data e hora da última modificação do dataSourceContainer.|
|releasedDateTime|DateTimeOffset|Data e hora em que o dataSourceContainer foi liberado do caso.|
|status|String|Status mais recente do dataSourceContainer. Os valores possíveis são: `Active`, `Released`.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.dataSourceContainer",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.dataSourceContainer",
  "id": "String (identifier)",
  "status": "String",
  "holdStatus": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "releasedDateTime": "String (timestamp)",
  "displayName": "String",
  "createdDateTime": "String (timestamp)"
}
```

