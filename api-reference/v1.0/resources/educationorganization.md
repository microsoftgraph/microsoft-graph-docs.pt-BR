---
title: tipo de recurso educationOrganization
description: Entidade abstrata usada para modelar a semelhança entre diferentes tipos de organização no setor educacional.
author: mlafleur
ms.localizationpriority: medium
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 047522db1552f6b48e21868235e3740abe7e6643
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59123696"
---
# <a name="educationorganization-resource-type"></a>tipo de recurso educationOrganization

Namespace: microsoft.graph

Entidade abstrata usada para modelar a semelhança entre diferentes tipos de organização no setor educacional.

Herda da [entidade](../resources/entity.md).

## <a name="properties"></a>Propriedades

| Propriedade             | Tipo                    | Descrição                                                                            |
| :------------------- | :---------------------- | :------------------------------------------------------------------------------------- |
| description          | String                  | Descrição da organização.                                                              |
| displayName          | Cadeia de caracteres                  | Nome de exibição da organização.                                                             |
| externalSource       | educationExternalSource | Fonte de onde essa organização foi criada. Os valores possíveis são: `sis` e `manual`. |
| externalSourceDetail | Cadeia de caracteres                  | O nome da fonte externa de onde esses recursos foram gerados.                     |
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
