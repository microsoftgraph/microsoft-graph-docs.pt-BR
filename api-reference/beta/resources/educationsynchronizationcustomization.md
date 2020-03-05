---
title: tipo de recurso educationSynchronizationCustomization
description: 'Fornece configurações para personalizar a sincronização do perfil de dados da escola das entidades de recurso. A personalização pode ser aplicada a todas as entidades que estão sendo sincronizadas. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 368117a5293f4ede59282fa1ced12d024976de52
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42500461"
---
# <a name="educationsynchronizationcustomization-resource-type"></a>tipo de recurso educationSynchronizationCustomization

Namespace: Microsoft. Graph

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
