---
title: Tipo de recurso bookingCustomQuestion
description: Representa uma pergunta personalizada para um bookingBusiness.
author: razortbone
ms.localizationpriority: medium
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 9a9f88d7ee5fe20d1dc5b4033353b2ac7b744878
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/15/2021
ms.locfileid: "61524995"
---
# <a name="bookingcustomquestion-resource-type"></a>Tipo de recurso bookingCustomQuestion

Namespace: microsoft.graph

Representa uma pergunta personalizada para [um bookingBusiness](bookingbusiness.md).

## <a name="methods"></a>Methods

| Método                                                                         | Tipo de retorno                                                               | Descrição                                                                                                       |
| :----------------------------------------------------------------------------- | :------------------------------------------------------------------------ | :---------------------------------------------------------------------------------------------------------------- |
| [Listar bookingCustomQuestions](../api/bookingbusiness-list-customquestions.md)  | [coleção bookingCustomQuestion](../resources/bookingcustomquestion.md) | Obter uma lista dos objetos [bookingCustomQuestion](../resources/bookingcustomquestion.md) e suas propriedades.    |
| [Criar bookingCustomQuestion](../api/bookingbusiness-post-customquestions.md) | [bookingCustomQuestion](../resources/bookingcustomquestion.md)            | Crie um novo [objeto bookingCustomQuestion.](../resources/bookingcustomquestion.md)                               |
| [Obter bookingCustomQuestion](../api/bookingcustomquestion-get.md)               | [bookingCustomQuestion](../resources/bookingcustomquestion.md)            | Leia as propriedades e as relações de um [objeto bookingCustomQuestion.](../resources/bookingcustomquestion.md) |
| [Atualizar bookingCustomQuestion](../api/bookingcustomquestion-update.md)         | [bookingCustomQuestion](../resources/bookingcustomquestion.md)            | Atualize as propriedades de um [objeto bookingCustomQuestion.](../resources/bookingcustomquestion.md)                 |
| [Excluir bookingCustomQuestion](../api/bookingcustomquestion-delete.md)         | Nenhuma                                                                      | [Exclua um objeto bookingCustomQuestion.](../resources/bookingcustomquestion.md)                                  |

## <a name="properties"></a>Propriedades

| Propriedade        | Tipo              | Descrição                                                                                               |
| :-------------- | :---------------- | :-------------------------------------------------------------------------------------------------------- |
| answerInputType | answerInputType   | O tipo de resposta esperado. Os valores possíveis são: `text`, `radioButton`, `unknownFutureValue`.     |
| answerOptions   | Coleção de cadeias de caracteres | Lista de valores de resposta possíveis.                                                                    |
| displayName     | Cadeia de caracteres            | A pergunta. |
| id              | Cadeia de caracteres            | A ID da pergunta personalizada. Herdado da [entidade](../resources/entity.md).                           |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.bookingCustomQuestion",
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
