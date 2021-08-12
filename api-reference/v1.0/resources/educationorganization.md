---
title: tipo de recurso educationOrganization
description: Entidade abstrata usada para modelar a semelhança entre diferentes tipos de organização no setor educacional.
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: fa6d324602ba13ebe186bc0631de991e193d945757117217aa29296ee480ef74
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54130349"
---
# <a name="educationorganization-resource-type"></a>tipo de recurso educationOrganization

Namespace: microsoft.graph

Entidade abstrata usada para modelar a semelhança entre diferentes tipos de organização no setor educacional.

Herda da [entidade](../resources/entity.md).

## <a name="properties"></a>Propriedades

| Propriedade             | Tipo                    | Descrição                                                                            |
| :------------------- | :---------------------- | :------------------------------------------------------------------------------------- |
| description          | Cadeia de caracteres                  | Descrição da organização.                                                              |
| displayName          | Cadeia de caracteres                  | Nome de exibição da organização.                                                             |
| externalSource       | educationExternalSource | Fonte de onde essa organização foi criada. Os valores possíveis são: `sis` e `manual`. |
| externalSourceDetail | String                  | O nome da fonte externa de onde esses recursos foram gerados.                     |
| id                   | Cadeia de caracteres                  | Identificador de objeto. Herdado da [entidade](../resources/entity.md)                     |

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
