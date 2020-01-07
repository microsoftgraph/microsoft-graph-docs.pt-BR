---
title: tipo de recurso shiftPreferences
description: Representa a disponibilidade de um usuário a ser atribuída a turnos no cronograma.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 083b0ad81ffee25d8a03bf5ff38815d2ca0155a8
ms.sourcegitcommit: ed03445225e98cf0881de08273c36be8d0e576ea
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/07/2020
ms.locfileid: "40952269"
---
# <a name="shiftpreferences-resource-type"></a>tipo de recurso shiftPreferences

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa a disponibilidade de um usuário a ser atribuída a turnos no [cronograma](schedule.md).

## <a name="methods"></a>Methods

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Get](../api/shiftpreferences-get.md) | [shiftPreferences](shiftpreferences.md) | Leia as propriedades e os relacionamentos de um objeto **shiftPreferences** . |
| [Update](../api/shiftpreferences-put.md) | [shiftPreferences](shiftpreferences.md) | Atualizar um objeto **shiftPreferences** . |

## <a name="properties"></a>Propriedades

|Propriedade          |Tipo           |Descrição                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| id | `Edm.String` | O identificador da entidade. |
| @odata.etag | `Edm.String` | A chave de alteração da entidade. |
| availability | coleção [shiftAvailability](shiftavailability.md) | Disponibilidade do usuário a ser agendada para trabalho e seu padrão de recorrência. |
| createdDateTime | `Edm.DateTimeOffset` | Carimbo de data/hora correspondente a quando a entidade foi criada. |
| lastModifiedDateTime | `Edm.DateTimeOffset` | Carimbo de data/hora correspondente a quando a entidade foi modificada pela última vez. |
| lastModifiedBy | [identitySet](identityset.md) | Identidade da pessoa que modificou a entidade pela última vez. |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.shiftPreferences",
  "baseType": "microsoft.graph.changeTrackedEntity"
}-->

```json
{
  "availability": [{"@odata.type": "microsoft.graph.shiftAvailability"}]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "shiftPreferences resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
