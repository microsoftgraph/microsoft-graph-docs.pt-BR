---
title: tipo de recurso dataSource
description: Entidade DataSource-classe base abstrata
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: 645ae33eb6c43972122623e52bfecf17f39491e4
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597530"
---
# <a name="datasource-resource-type"></a>tipo de recurso dataSource

Namespace: Microsoft Graph

A entidade dataSource é uma BaseClass abstrata usada para identificar fontes de conteúdo para descoberta eletrônica.

## <a name="methods"></a>Methods

Nenhum

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|createdBy|[identitySet](../resources/identityset.md)|O usuário que criou a **fonte** de os.|
|createdDateTime|DateTimeOffset|A data e a hora em que a **fonte** de dados foi criada.|
|displayName|String|O nome de exibição da **fonte de fontes**. Este será o nome do site do SharePoint.|
|id|String| A ID da **DataSource**. Esta não é a ID do site real.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.dataSource",
  "baseType": "",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.dataSource",
  "displayName": "String",
  "createdDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "id": "String (identifier)"
}
```
