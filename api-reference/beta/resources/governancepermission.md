---
title: Tipo de recurso governancePermission
description: 'Representa a permissão de acesso que um governanceSubject tem para um governanceResource específico.  '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu1
ms.openlocfilehash: c094050f32b020c204d645dfc0c398ad5bfa5d20
ms.sourcegitcommit: 01755ac7c0ab7becf28052e05e58567caa8364cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/21/2021
ms.locfileid: "58453727"
---
# <a name="governancepermission-resource-type"></a>Tipo de recurso governancePermission

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa a permissão de acesso que [um governanceSubject](../resources/governancesubject.md) tem para uma [governança EspecíficaResource](../resources/governanceresource.md).


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|accessLevel|Cadeia de caracteres|O nível de acesso. Valores válidos: ``None`` ``UserRead`` , , e ``AdminRead`` ``AdminReadWrite`` .|
|isActive|Booliano|Indique se o solicitante tem qualquer atribuição de função ativa para o nível de acesso.|
|isEligible|Booliano|Indique se o solicitante tem qualquer atribuição de função qualificada para o nível de acesso.|

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


