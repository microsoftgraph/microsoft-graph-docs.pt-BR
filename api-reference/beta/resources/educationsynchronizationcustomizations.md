---
title: tipo de recurso de educationSynchronizationCustomizations
description: Contém a lista de entidades de sincronização e suas personalizações, se houver alguma.
ms.openlocfilehash: d694c5ea1136d38e11ff3f1aca0ad0fde34b9d02
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037405"
---
# <a name="educationsynchronizationcustomizations-resource-type"></a>tipo de recurso de educationSynchronizationCustomizations

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Contém a lista de entidades de sincronização e suas [personalizações](educationsynchronizationcustomization.md), se houver alguma.

> **Observação:** Personalização das propriedades para sincronizar não se aplica às entidades **studentEnrollment** e **teacherRoster** .

Este recurso é membro dos provedores de dados a seguir:

* [educationCsvDataProvider](educationcsvdataprovider.md)
* [educationPowerSchoolDataProvider](educationpowerschooldataprovider.md)

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:-|:-|:-|
| **escola** | [educationSynchronizationCustomization](educationsynchronizationcustomization.md) |  Personalização para uma entidade escola.        |
| **section** | [educationSynchronizationCustomization](educationsynchronizationcustomization.md) |  Personalização para uma entidade de seção.         |
| **student** | [educationSynchronizationCustomization](educationsynchronizationcustomization.md) |  Personalização para uma entidade de student.         |
| **teacher** | [educationSynchronizationCustomization](educationsynchronizationcustomization.md) |  Personalização para uma entidade de professor.         |
| **studentEnrollment** | [educationSynchronizationCustomization](educationsynchronizationcustomization.md) |  Personalização para o registro de student.           |
| **teacherRoster** | [educationSynchronizationCustomization](educationsynchronizationcustomization.md) |       Personalização para uma lista de participação do professor.    |

## <a name="json-representation"></a>Representação JSON
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationSynchronizationCustomizations"
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
