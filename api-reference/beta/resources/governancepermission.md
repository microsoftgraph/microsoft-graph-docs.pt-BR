---
title: Tipo de recurso governancePermission
description: 'Representa a permissão de acesso que um governanceSubject tem para um governanceResource específico.  '
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: japere
ms.openlocfilehash: b4244335bba57c9ff5200099520e2e0b2a5e98c2
ms.sourcegitcommit: 43a7c971a97ce1e4c55cbae089820bfce7dfe42b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2022
ms.locfileid: "64510405"
---
# <a name="governancepermission-resource-type"></a>Tipo de recurso governancePermission

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [pim-v2ResourceRoles-deprecation](../../includes/pim-v2ResourceRoles-deprecation.md)]

Representa a permissão de acesso que [um governanceSubject](../resources/governancesubject.md) tem para um [governanceResource específico](../resources/governanceresource.md).


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|accessLevel|Cadeia de caracteres|O nível de acesso. Valores válidos: ``None``, ``UserRead``, ``AdminRead``e ``AdminReadWrite``.|
|isActive|Boolean|Indique se o solicitante tem qualquer atribuição de função ativa para o nível de acesso.|
|isEligible|Boolean|Indique se o solicitante tem qualquer atribuição de função qualificada para o nível de acesso.|

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


