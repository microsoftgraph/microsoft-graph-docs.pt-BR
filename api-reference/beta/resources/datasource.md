---
title: Tipo de recurso dataSource
description: Entidade Datasource - classe base abstrata
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: c019a6b8338180584a31382c0741018791973184
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161919"
---
# <a name="datasource-resource-type"></a>Tipo de recurso dataSource

Namespace: microsoft.graph

A entidade dataSource é uma baseclass abstrata usada para identificar fontes de conteúdo para Descobertas e Descobertas.

## <a name="methods"></a>Métodos

Nenhum(a)

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|createdBy|[identitySet](../resources/identityset.md)|O usuário que criou **o dataSource**.|
|createdDateTime|DateTimeOffset|A data e a hora em **que o dataSource** foi criado.|
|displayName|String|O nome de exibição **do dataSource**. Esse será o nome do site do SharePoint.|
|id|String| A ID do **dataSource**. Essa não é a ID do site real.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.dataSource",
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
