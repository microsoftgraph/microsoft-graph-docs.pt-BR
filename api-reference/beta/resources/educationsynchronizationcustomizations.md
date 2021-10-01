---
title: tipo de recurso educationSynchronizationCustomizations
description: Contém a lista de entidades para sincronizar e suas personalizações, se alguma.
ms.localizationpriority: medium
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 30792f67b04606235a99e131d58ffb72bebe8ebd
ms.sourcegitcommit: 0ec845f93eaa140ad833ba163c76c5308197a92f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/01/2021
ms.locfileid: "60068584"
---
# <a name="educationsynchronizationcustomizations-resource-type"></a>tipo de recurso educationSynchronizationCustomizations

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contém a lista de entidades para sincronizar e suas personalizações, se alguma.

> [!NOTE]
> A personalização de propriedades para sincronização não se aplica às Inscrições de Alunos ou Às Listas de Professores.

Esse recurso é membro dos seguintes provedores de dados:

- [educationCsvDataProvider](educationcsvdataprovider.md)
- [educationPowerSchoolDataProvider](educationpowerschooldataprovider.md)

## <a name="properties"></a>Propriedades

| Propriedade          | Tipo                                    | Descrição                             |
| :---------------- | :-------------------------------------- | :-------------------------------------- |
| school            | [educationSynchronizationCustomization] | Personalizações para entidades escolares.     |
| section           | [educationSynchronizationCustomization] | Personalizações para entidades de seção.    |
| student           | [educationSynchronizationCustomization] | Personalizações para entidades de alunos.    |
| teacher           | [educationSynchronizationCustomization] | Personalizações para entidades de professores.    |
| studentEnrollment | [educationSynchronizationCustomization] | Personalizações para inscrições de alunos. |
| teacherRoster     | [educationSynchronizationCustomization] | Personalizações para Lista de Professores.     |

[educationsynchronizationcustomization]: educationsynchronizationcustomization.md

## <a name="json-representation"></a>Representação JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type&quot;: &quot;microsoft.graph.educationSynchronizationCustomizations"
}-->

```json
{
  "school": {
    "@odata.type": "microsoft.graph.educationSynchronizationCustomization",
    "optionalPropertiesToSync": ["String"],
    "isSyncDeferred": "Boolean",
    "allowDisplayNameUpdate&quot;: &quot;Boolean"
  },
  "section": {
    "@odata.type": "microsoft.graph.educationSynchronizationCustomization",
    "optionalPropertiesToSync": ["String"],
    "isSyncDeferred": "Boolean",
    "allowDisplayNameUpdate&quot;: &quot;Boolean"
  },
  "student": {
    "@odata.type": "microsoft.graph.educationSynchronizationCustomization",
    "optionalPropertiesToSync": ["String"],
    "isSyncDeferred": "Boolean",
    "allowDisplayNameUpdate&quot;: &quot;Boolean"
  },
  "teacher": {
    "@odata.type": "microsoft.graph.educationSynchronizationCustomization",
    "optionalPropertiesToSync": ["String"],
    "isSyncDeferred": "Boolean",
    "allowDisplayNameUpdate&quot;: &quot;Boolean"
  },
  "studentEnrollment": {
    "@odata.type": "microsoft.graph.educationSynchronizationCustomization",
    "synchronizationStartDate": "DateTimeOffset",
    "isSyncDeferred": "Boolean",
    "allowDisplayNameUpdate&quot;: &quot;Boolean"
  },
  "teacherRoster": {
    "@odata.type": "microsoft.graph.educationSynchronizationCustomization",
    "isSyncDeferred": "Boolean",
    "allowDisplayNameUpdate&quot;: &quot;Boolean"
  }
}
```


