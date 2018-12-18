---
title: tipo de recurso de educationSynchronizationCustomization
description: 'Fornece configurações para personalizar a sincronização de perfil de dados da escola das entidades que recurso. A personalização pode ser aplicada a todas as entidades que está sendo sincronizadas. '
author: mmast-msft
ms.openlocfilehash: d4f67c9f56198350731c18fe3da8b512522c4d71
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27350633"
---
# <a name="educationsynchronizationcustomization-resource-type"></a>tipo de recurso de educationSynchronizationCustomization

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Fornece configurações para personalizar a sincronização de perfil de dados da escola das entidades que recurso. A personalização pode ser aplicada a todas as entidades que está sendo sincronizadas. 

>**Observação:** A propriedade **synchronizationStartDate** só se aplica à entidade **StudentEnrollment** .

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:-|:-|:-|
| **optionalPropertiesToSync** | coleção de cadeia de caracteres |  A coleção de nomes de propriedade para sincronização. Se definido como nulo, todas as propriedades serão sincronizados.       |
| **synchronizationStartDate** | DateTime |  A data em que a sincronização deve ser iniciado. Este valor deve ser definido como uma data futura. Se definido como null, o recurso será sincronizado após a conclusão da configuração do perfil. **Observação:** Isso se aplica apenas à propriedade **StudentEnrollment** .      |
|**isSyncDeferred** |Boolean | Indica se a sincronização da entidade pai é adiada para uma data posterior. |
| **allowDisplayNameUpdate** | Boolean |  Indica se o nome de exibição do recurso pode ser substituído pela sincronização.         |


## <a name="json-representation"></a>Representação JSON
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationSynchronizationCustomization"
}-->

```json
{  
    "optionalPropertiesToSync":["String"],
    "synchronizationStartDate": "DateTimeOffset",
    "isSyncDeferred": "Boolean",
    "allowDisplayNameUpdate": "Boolean"
}
```
