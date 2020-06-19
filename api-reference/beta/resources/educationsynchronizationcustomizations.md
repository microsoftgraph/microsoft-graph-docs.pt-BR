---
title: tipo de recurso educationSynchronizationCustomizations
description: Contém a lista de entidades a serem sincronizadas e suas personalizações, se houver.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 6df720b8f0e02ba24f3972833a6a76219d327925
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44790926"
---
# <a name="educationsynchronizationcustomizations-resource-type"></a>tipo de recurso educationSynchronizationCustomizations

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contém a lista de entidades a serem sincronizadas e suas personalizações, se houver.

> [!NOTE]
> A personalização das propriedades a serem sincronizadas não se aplica às registradoras ou às listas de professores do aluno.

Este recurso é membro dos seguintes provedores de dados:

- [educationCsvDataProvider](educationcsvdataprovider.md)
- [educationPowerSchoolDataProvider](educationpowerschooldataprovider.md)

## <a name="properties"></a>Propriedades

| Propriedade          | Tipo                                    | Descrição                             |
| :---------------- | :-------------------------------------- | :-------------------------------------- |
| escola            | [educationSynchronizationCustomization] | Personalizações para entidades escolares.     |
| section           | [educationSynchronizationCustomization] | Personalizações para entidades de seção.    |
| student           | [educationSynchronizationCustomization] | Personalizações para entidades de alunos.    |
| teacher           | [educationSynchronizationCustomization] | Personalizações para entidades de professores.    |
| studentEnrollment | [educationSynchronizationCustomization] | Personalizações para o registro de alunos. |
| teacherRoster     | [educationSynchronizationCustomization] | Personalizações para as listas de professores.     |

[educationsynchronizationcustomization]: educationsynchronizationcustomization.md

## <a name="json-representation"></a>Representação JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationCustomizations"
}-->

```json
{
  "school": {
    "@odata.type": "microsoft.graph.educationSynchronizationCustomization"
  },
  "section": {
    "@odata.type": "microsoft.graph.educationSynchronizationCustomization"
  },
  "student": {
    "@odata.type": "microsoft.graph.educationSynchronizationCustomization"
  },
  "teacher": {
    "@odata.type": "microsoft.graph.educationSynchronizationCustomization"
  },
  "studentEnrollment": {
    "@odata.type": "microsoft.graph.educationSynchronizationCustomization"
  },
  "teacherRoster": {
    "@odata.type": "microsoft.graph.educationSynchronizationCustomization"
  }
}
```
