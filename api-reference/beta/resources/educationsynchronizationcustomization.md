---
title: tipo de recurso de educationSynchronizationCustomization
description: 'Fornece configurações para personalizar a sincronização de perfil de dados da escola das entidades que recurso. A personalização pode ser aplicada a todas as entidades que está sendo sincronizadas. '
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: 9294af5796daeefb394ed1625a9a36128ae7b2a4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860897"
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
|**isSyncDeferred** |Booliano | Indica se a sincronização da entidade pai é adiada para uma data posterior. |
| **allowDisplayNameUpdate** | Booliano |  Indica se o nome de exibição do recurso pode ser substituído pela sincronização.         |


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
