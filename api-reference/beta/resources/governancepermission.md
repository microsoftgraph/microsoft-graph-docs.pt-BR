---
title: tipo de recurso governancePermission
description: 'Representa a permissão de acesso que um governanceSubject tem a um Entidadegovernanceresource específico.  '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 8bf32b855ed77ccdf712b1a739ef913d0a3dade0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35971939"
---
# <a name="governancepermission-resource-type"></a>tipo de recurso governancePermission

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa a permissão de acesso que um [governanceSubject](../resources/governancesubject.md) tem a um [entidadegovernanceresource](../resources/governanceresource.md)específico.  


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|accessLevel|String|O nível de acesso. Valores válidos: ``None``, ``UserRead``, ``AdminRead``e ``AdminReadWrite``.|
|isActive|Booliano|Indica se o solicitante tem qualquer atribuição de função ativa para o nível de acesso.|
|isqualificável|Booliano|Indica se o solicitante tem qualquer atribuição de função qualificada para o nível de acesso.|

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
