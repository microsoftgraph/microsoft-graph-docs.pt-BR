---
title: Tipo de recurso bookingCustomQuestion
description: Representa uma pergunta personalizada para um bookingBusiness.
author: razortbone
ms.localizationpriority: medium
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: cf672b93e30b6351d3f543b5cc9341d53fea1d5d
ms.sourcegitcommit: 8253b79a9fdfea723899860492219eaeb9f74e3d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2022
ms.locfileid: "66160633"
---
# <a name="bookingcustomquestion-resource-type"></a>Tipo de recurso bookingCustomQuestion

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma pergunta personalizada para [um bookingBusiness](bookingbusiness.md).

Herda de [bookingNamedEntity](../resources/bookingnamedentity.md).

## <a name="methods"></a>Métodos

| Método                                                                         | Tipo de retorno                                                               | Descrição                                                                                                       |
| :----------------------------------------------------------------------------- | :------------------------------------------------------------------------ | :---------------------------------------------------------------------------------------------------------------- |
| [Listar bookingCustomQuestions](../api/bookingbusiness-list-customquestions.md)            | [coleção bookingCustomQuestion](../resources/bookingcustomquestion.md) | Obtenha uma lista dos objetos [bookingCustomQuestion](../resources/bookingcustomquestion.md) e suas propriedades.    |
| [Criar bookingCustomQuestion](../api/bookingbusiness-post-customquestions.md) | [bookingCustomQuestion](../resources/bookingcustomquestion.md)            | Crie um novo [objeto bookingCustomQuestion](../resources/bookingcustomquestion.md) .                               |
| [Obter bookingCustomQuestion](../api/bookingcustomquestion-get.md)               | [bookingCustomQuestion](../resources/bookingcustomquestion.md)            | Leia as propriedades e as relações de um [objeto bookingCustomQuestion](../resources/bookingcustomquestion.md) . |
| [Atualizar bookingCustomQuestion](../api/bookingcustomquestion-update.md)         | Nenhuma     | Atualize as propriedades de um [objeto bookingCustomQuestion](../resources/bookingcustomquestion.md) .                 |
| [Excluir bookingCustomQuestion](../api/bookingcustomquestion-delete.md)         | Nenhuma                                                                      | [Exclua um objeto bookingCustomQuestion](../resources/bookingcustomquestion.md).                                  |

## <a name="properties"></a>Propriedades

| Propriedade        | Tipo              | Descrição                                                                                               |
| :-------------- | :---------------- | :-------------------------------------------------------------------------------------------------------- |
| answerInputType | answerInputType   | O tipo de resposta esperado. Os valores possíveis são: `text`, `radioButton`, `unknownFutureValue`.     |
| answerOptions   | Coleção String | Lista de possíveis valores de resposta.                                                                    |
| displayName     | Cadeia de caracteres            | A pergunta. Herdado de [bookingNamedEntity](../resources/bookingnamedentity.md). |
| id              | Cadeia de caracteres            | A ID da pergunta personalizada. Herdado da [entidade](../resources/entity.md).                           |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.bookingCustomQuestion",
  "baseType": "microsoft.graph.bookingNamedEntity",
  "openType": false
}
-->

```json
{
  "@odata.type": "#microsoft.graph.bookingCustomQuestion",
  "id": "String (identifier)",
  "displayName": "String",
  "answerInputType": {"@odata.type": "microsoft.graph.answerInputType"},
  "answerOptions": ["String"]
}
```
