---
title: Tipo de recurso shiftPreferences
description: Representa a disponibilidade de um usuário a ser atribuído turnos na agenda.
ms.localizationpriority: medium
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: d9bebb27005d18e6fa94673a449a47f8d40f23d7
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59032157"
---
# <a name="shiftpreferences-resource-type"></a>Tipo de recurso shiftPreferences

Namespace: microsoft.graph

Representa a disponibilidade de um usuário a ser atribuída a turnos na [agenda](schedule.md).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Get](../api/shiftpreferences-get.md) | [shiftPreferences](shiftpreferences.md) | Leia as propriedades e as relações de um **objeto shiftPreferences.** |
| [Atualizar](../api/shiftpreferences-put.md) | [shiftPreferences](shiftpreferences.md) | Atualize um **objeto shiftPreferences.** |

## <a name="properties"></a>Propriedades

|Propriedade          |Tipo           |Descrição                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| id | `Edm.String` | O identificador da entidade. |
| @odata.etag | `Edm.String` | A chave de alteração da entidade. |
| availability | [Coleção shiftAvailability](shiftavailability.md) | Disponibilidade do usuário a ser agendado para o trabalho e seu padrão de recorrência. |
| createdDateTime | `Edm.DateTimeOffset` | Timestamp correspondente a quando a entidade foi criada. |
| lastModifiedDateTime | `Edm.DateTimeOffset` | Timestamp correspondente a quando a entidade foi modificada pela última vez. |
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

