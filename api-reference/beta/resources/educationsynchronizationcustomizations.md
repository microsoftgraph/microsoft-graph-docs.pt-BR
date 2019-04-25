---
title: tipo de recurso educationSynchronizationCustomizations
description: Contém a lista de entidades a serem sincronizadas e suas personalizações, se houver.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 9e513e64afb1478ca7b5cc5d53f1964d16d9928b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543188"
---
# <a name="educationsynchronizationcustomizations-resource-type"></a>tipo de recurso educationSynchronizationCustomizations

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contém a lista de entidades a serem sincronizadas [](educationsynchronizationcustomization.md)e suas personalizações, se houver.

> **Observação:** A personalização das propriedades a serem sincronizadas não se aplica às entidades **studentEnrollment** e **teacherRoster** .

Este recurso é membro dos seguintes provedores de dados:

* [educationCsvDataProvider](educationcsvdataprovider.md)
* [educationPowerSchoolDataProvider](educationpowerschooldataprovider.md)

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:-|:-|:-|
| **escola** | [educationSynchronizationCustomization](educationsynchronizationcustomization.md) |  Personalização de uma entidade escolar.        |
| **section** | [educationSynchronizationCustomization](educationsynchronizationcustomization.md) |  Personalização de uma entidade de seção.         |
| **student** | [educationSynchronizationCustomization](educationsynchronizationcustomization.md) |  Personalização de uma entidade de aluno.         |
| **teacher** | [educationSynchronizationCustomization](educationsynchronizationcustomization.md) |  Personalização de uma entidade professor.         |
| **studentEnrollment** | [educationSynchronizationCustomization](educationsynchronizationcustomization.md) |  Personalização para registro de alunos.           |
| **teacherRoster** | [educationSynchronizationCustomization](educationsynchronizationcustomization.md) |       Personalização de uma lista de professores.    |

## <a name="json-representation"></a>Representação JSON
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationCustomizations"
}-->

```json
{
  "school": {"@odata.type": "microsoft.graph.educationSynchronizationCustomization"},
  "section": {"@odata.type": "microsoft.graph.educationSynchronizationCustomization"},
  "student": {"@odata.type": "microsoft.graph.educationSynchronizationCustomization"},
  "teacher": {"@odata.type": "microsoft.graph.educationSynchronizationCustomization"},
  "studentEnrollment": {"@odata.type": "microsoft.graph.educationSynchronizationCustomization"},
  "teacherRoster": {"@odata.type": "microsoft.graph.educationSynchronizationCustomization"}
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsynchronizationcustomizations.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
