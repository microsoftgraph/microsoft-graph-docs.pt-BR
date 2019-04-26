---
title: tipo de recurso educationSynchronizationCustomizations
description: Contém a lista de entidades a serem sincronizadas e suas personalizações, se houver.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 0d1a886557e37bb19b23c5e0c1d74b937112cc58
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334098"
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
