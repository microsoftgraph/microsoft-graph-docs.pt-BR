---
title: Tipo de recurso dataSource
description: A entidade dataSource é uma classe base abstrata usada para identificar fontes de conteúdo para Descoberta Eletrônica.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: c388280b0c6c8f005c59dcdfb11aa20fafa18dbd
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/18/2022
ms.locfileid: "66839244"
---
# <a name="datasource-resource-type"></a>Tipo de recurso dataSource

Namespace: microsoft.graph.security



A entidade dataSource é uma classe base abstrata usada para identificar fontes de conteúdo para Descoberta Eletrônica.

## <a name="methods"></a>Métodos

Nenhum.
## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|createdBy|[identitySet](../resources/identityset.md)|O usuário que criou **o dataSource**.|
|createdDateTime|DateTimeOffset|A data e a hora em **que a fonte de dados** foi criada.|
|displayName|String|O nome de exibição **do dataSource**. Esse será o nome do site do SharePoint.|
|id|Cadeia de caracteres| A ID da **fonte de dados**. Essa não é a ID do site real.|
|holdStatus|microsoft.graph.security.dataSourceHoldStatus|O status de retenção do **dataSource**. Os valores possíveis são: `notApplied`, `applied`, `applying`, , `removing``partial`|
## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.dataSource",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.dataSource",
  "id": "String (identifier)",
  "displayName": "String",
  "holdStatus": "String",
  "createdDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```

