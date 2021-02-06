---
title: Tipo de recurso governancePermission
description: 'Representa a permissão de acesso que um governanceSubject tem para uma governanceResource específica.  '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: f316a863ecba9ed546b9ba4045e57ada87e97ab9
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50128831"
---
# <a name="governancepermission-resource-type"></a>Tipo de recurso governancePermission

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa a permissão de acesso que um [governanceSubject](../resources/governancesubject.md) tem para uma [governança EspecíficaResource](../resources/governanceresource.md).


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|accessLevel|String|O nível de acesso. Valores válidos: ``None`` ``UserRead`` , , e ``AdminRead`` ``AdminReadWrite`` .|
|isActive|Boolean|Indica se o solicitante tem qualquer atribuição de função ativa para o nível de acesso.|
|isEligible|Boolean|Indica se o solicitante tem qualquer atribuição de função qualificada para o nível de acesso.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.governancePermission"
}-->
```json
{
  "accessLevel": "String",
  "isActive": true,
  "isEligible": true
}

```


