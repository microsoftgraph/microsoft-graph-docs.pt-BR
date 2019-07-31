---
title: tipo de recurso educationSynchronizationCustomizations
description: Contém a lista de entidades a serem sincronizadas e suas personalizações, se houver.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: d31be9bd808f411c1e208ab953784fdefd65fdda
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972436"
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
