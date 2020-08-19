---
title: tipo de recurso governancePermission
description: 'Representa a permissão de acesso que um governanceSubject tem a um Entidadegovernanceresource específico.  '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: shauliu
ms.openlocfilehash: 113f25cd276cf01ce46e3c410ca4b5b409417d98
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46809513"
---
# <a name="governancepermission-resource-type"></a>tipo de recurso governancePermission

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa a permissão de acesso que um [governanceSubject](../resources/governancesubject.md) tem a um [entidadegovernanceresource](../resources/governanceresource.md)específico.


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|accessLevel|String|O nível de acesso. Valores válidos: ``None`` , ``UserRead`` , ``AdminRead`` e ``AdminReadWrite`` .|
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
