---
title: tipo de recurso de educationSynchronizationCustomizations
description: Contém a lista de entidades de sincronização e suas personalizações, se houver alguma.
localization_priority: Normal
ms.openlocfilehash: 0c07b166c09b2bfa6bf88159533523dab869a325
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27817035"
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
