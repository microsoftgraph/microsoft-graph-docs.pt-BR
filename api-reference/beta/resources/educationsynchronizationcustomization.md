---
title: tipo de recurso educationSynchronizationCustomization
description: 'Fornece configurações para personalizar a sincronização do perfil de dados da escola das entidades de recurso. A personalização pode ser aplicada a todas as entidades que estão sendo sincronizadas. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 397f4d732bc25d086b2aeae6efc697d2048e6a03
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334090"
---
# <a name="educationsynchronizationcustomization-resource-type"></a>tipo de recurso educationSynchronizationCustomization

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Fornece configurações para personalizar a sincronização do perfil de dados da escola das entidades de recurso. A personalização pode ser aplicada a todas as entidades que estão sendo sincronizadas. 

>**Observação:** A propriedade **synchronizationStartDate** só se aplica à entidade **StudentEnrollment** .

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:-|:-|:-|
| **optionalPropertiesToSync** | coleção de cadeia de caracteres |  A coleção de nomes de propriedade a serem sincronizados. Se definido como nulo, todas as propriedades serão sincronizadas.       |
| **synchronizationStartDate** | DateTime |  A data em que a sincronização deve ser iniciada. Esse valor deve ser definido para uma data futura. Se definido como nulo, o recurso será sincronizado quando a configuração do perfil for concluída. **Observação:** Isso só se aplica à propriedade **StudentEnrollment** .      |
|**isSyncDeferred** |Boolean | Indica se a sincronização da entidade pai será adiada para uma data posterior. |
| **allowDisplayNameUpdate** | Boolean |  Indica se o nome de exibição do recurso pode ser substituído pela sincronização.         |


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
