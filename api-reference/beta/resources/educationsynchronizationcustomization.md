---
title: tipo de recurso educationSynchronizationCustomization
description: 'Fornece configurações para personalizar a sincronização do perfil de dados da escola das entidades de recurso. A personalização pode ser aplicada a todas as entidades que estão sendo sincronizadas. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: c3f704339dbf2acbe7cb78e1899c5f209f50f21e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48055587"
---
# <a name="educationsynchronizationcustomization-resource-type"></a>tipo de recurso educationSynchronizationCustomization

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Fornece configurações para personalizar a sincronização do perfil de dados da escola das entidades de recurso. A personalização pode ser aplicada a todas as entidades que estão sendo sincronizadas.

## <a name="properties"></a>Propriedades

| Propriedade                 | Tipo              | Descrição                                                                                                                                                                                                            |
| :----------------------- | :---------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| optionalPropertiesToSync | Coleção de cadeias de caracteres | A coleção de nomes de propriedade a serem sincronizados. Se definido como nulo, todas as propriedades serão sincronizadas. **Não se aplica a registradoras ou listas de professores do aluno**                                                            |
| synchronizationStartDate | DateTime          | A data em que a sincronização deve ser iniciada. Esse valor deve ser definido para uma data futura. Se definido como nulo, o recurso será sincronizado quando a configuração do perfil for concluída. **Aplica-se apenas às registradoras de alunos** |
| isSyncDeferred           | Booliano           | Indica se a sincronização da entidade pai será adiada para uma data posterior.                                                                                                                                    |
| allowDisplayNameUpdate   | Booliano           | Indica se o nome de exibição do recurso pode ser substituído pela sincronização.                                                                                                                                     |

## <a name="json-representation"></a>Representação JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationCustomization"
}-->

```json
{
  "optionalPropertiesToSync": ["String"],
  "synchronizationStartDate": "DateTimeOffset",
  "isSyncDeferred": "Boolean",
  "allowDisplayNameUpdate": "Boolean"
}
```


