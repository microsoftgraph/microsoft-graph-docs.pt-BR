---
title: Tipo de recurso governancePermission
description: 'Representa a permissão de acesso que um governanceSubject tem a uma governanceResource específica.  '
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: rkarim-ms
ms.openlocfilehash: b88900882ecceabcfe5101aa4564b88116df605f
ms.sourcegitcommit: d7efd03a6782da5e44b422c9016869c779d64add
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2022
ms.locfileid: "65397947"
---
# <a name="governancepermission-resource-type"></a>Tipo de recurso governancePermission

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [pim-v2ResourceRoles-deprecation](../../includes/pim-v2ResourceRoles-deprecation.md)]

Representa a permissão de acesso que [um governanceSubject](../resources/governancesubject.md) tem a uma [governanceResource específica](../resources/governanceresource.md).


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|Accesslevel|Cadeia de caracteres|O nível de acesso. Valores válidos: ``None``, ``UserRead``, ``AdminRead``e ``AdminReadWrite``.|
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


