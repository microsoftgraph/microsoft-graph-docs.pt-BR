---
title: Tipo de recurso dataSourceContainer
description: Classe base para fontes de dados custodiantes e não custodiais.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: f90a527ec47cc6b9e14e536a4f8da4841d6504c8
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/18/2022
ms.locfileid: "66838644"
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
|holdStatus|microsoft.graph.security.dataSourceHoldStatus|O status de retenção do dataSourceContainer.Os valores possíveis são: `notApplied`, `applied`, `applying`, , `removing``partial`|
|createdDateTime|DateTimeOffset|Data e hora criadas da entidade dataSourceContainer.|
|displayName|Cadeia de caracteres|Nome de exibição da entidade dataSourceContainer.|
|id|String|Identificador exclusivo do dataSourceContainer. Herdado da [entidade](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|Data e hora da última modificação do dataSourceContainer.|
|releasedDateTime|DateTimeOffset|Data e hora em que o dataSourceContainer foi liberado do caso.|
|status|microsoft.graph.security.dataSourceContainerStatus|Status mais recente do dataSourceContainer. Os valores possíveis são: `Active` e `Released`.|


### <a name="datasourcecontainerstatus-values"></a>Valores de dataSourceContainerStatus

|Member|Descrição|
|:----|-----------|
| Ativo| O contêiner de fonte de dados está ativo.|
| Lançamento | O contêiner de fonte de dados foi liberado.|

### <a name="datasourceholdstatus-values"></a>Valores de dataSourceHoldStatus

|Member|Descrição|
|:----|-----------|
| notApplied | O contêiner da fonte de dados não está em espera.|
| Aplicado | O contêiner da fonte de dados está em espera.|
| Aplicação | O contêiner de fonte de dados está aplicando o estado de retenção (operação applyHold disparada).|
| Remover | O contêiner de fonte de dados está removendo o estado de retenção (operação removeHold disparada).|
| Parcial | O contêiner de fonte de dados está em estado misto em que algumas fontes estão em espera e outras não estão em retenção ou estado de erro.|


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

