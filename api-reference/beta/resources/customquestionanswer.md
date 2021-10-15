---
title: Tipo de recurso customQuestionAnswer
description: Representa a resposta de um registro a uma pergunta de registro personalizada.
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
ms.date: 09/30/2021
doc_type: resourcePageType
ms.openlocfilehash: 4bed8b0c706f7ed1391465534213e849a9f0effe
ms.sourcegitcommit: c3f849e5a052b1926373a4b316ec303250e6d09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/15/2021
ms.locfileid: "60369447"
---
# <a name="customquestionanswer-resource-type"></a>Tipo de recurso customQuestionAnswer

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa a resposta de um registro à pergunta de registro [personalizada](meetingregistrationquestion.md) associada a [uma meetingRegistration](meetingregistration.md).

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
| :------- | :--- | :---------- |
| displayName | Cadeia de caracteres | Nome de exibição da pergunta de registro personalizado. Somente leitura. |
| questionId | Cadeia de caracteres | ID da pergunta de registro personalizado. Somente leitura.|
| value | Cadeia de caracteres | Responda à pergunta de registro personalizado. |

## <a name="json-representation"></a>Representação JSON

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.customQuestionAnswer"
}-->

```json
{
  "id": "String",
  "displayName": "String",
  "value": "String"
}
```
