---
title: tipo de recurso educationOrganization
description: Entidade abstrata usada para modelar a semelhança entre diferentes tipos de organização no setor educacional.
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: b24313b6b6061449faea0ecb4880a421a2333099
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52231861"
---
# <a name="educationorganization-resource-type"></a>tipo de recurso educationOrganization

Namespace: microsoft.graph

Entidade abstrata usada para modelar a semelhança entre diferentes tipos de organização no setor educacional.

Herda da [entidade](../resources/entity.md).

## <a name="properties"></a>Propriedades

| Propriedade             | Tipo                    | Descrição                                                                            |
| :------------------- | :---------------------- | :------------------------------------------------------------------------------------- |
| description          | String                  | Descrição da organização.                                                              |
| displayName          | String                  | Nome de exibição da organização.                                                             |
| externalSource       | educationExternalSource | Fonte de onde essa organização foi criada. Os valores possíveis são: `sis` e `manual`. |
| externalSourceDetail | String                  | O nome da fonte externa de onde esses recursos foram gerados.                     |
| id                   | String                  | Identificador de objeto. Herdado da [entidade](../resources/entity.md)                     |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.educationOrganization",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

```json
{
  "@odata.type": "#microsoft.graph.educationOrganization",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "externalSource": "String",
  "externalSourceDetail": "String"
}
```
