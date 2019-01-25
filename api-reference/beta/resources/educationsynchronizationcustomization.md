---
title: tipo de recurso de educationSynchronizationCustomization
description: 'Fornece configurações para personalizar a sincronização de perfil de dados da escola das entidades que recurso. A personalização pode ser aplicada a todas as entidades que está sendo sincronizadas. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 8af6c5e2173a8b04e730529123b4608fd236f959
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513603"
---
# <a name="educationsynchronizationcustomization-resource-type"></a>tipo de recurso de educationSynchronizationCustomization

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Fornece configurações para personalizar a sincronização de perfil de dados da escola das entidades que recurso. A personalização pode ser aplicada a todas as entidades que está sendo sincronizadas. 

>**Observação:** A propriedade **synchronizationStartDate** só se aplica à entidade **StudentEnrollment** .

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:-|:-|:-|
| **optionalPropertiesToSync** | Coleção de Cadeias de Caracteres |  A coleção de nomes de propriedade para sincronização. Se definido como nulo, todas as propriedades serão sincronizados.       |
| **synchronizationStartDate** | DateTime |  A data em que a sincronização deve ser iniciado. Este valor deve ser definido como uma data futura. Se definido como null, o recurso será sincronizado após a conclusão da configuração do perfil. **Observação:** Isso se aplica apenas à propriedade **StudentEnrollment** .      |
|**isSyncDeferred** |Booliano | Indica se a sincronização da entidade pai é adiada para uma data posterior. |
| **allowDisplayNameUpdate** | Booliano |  Indica se o nome de exibição do recurso pode ser substituído pela sincronização.         |


## <a name="json-representation"></a>Representação JSON
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationCustomization"
}-->

```json
{  
    "optionalPropertiesToSync":["String"],
    "synchronizationStartDate": "DateTimeOffset",
    "isSyncDeferred": "Boolean",
    "allowDisplayNameUpdate": "Boolean"
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsynchronizationcustomization.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
