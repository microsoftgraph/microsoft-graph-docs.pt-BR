---
title: Tipo de recurso bookingQuestionAnswer
description: Contém uma pergunta personalizada, a resposta dada pelo cliente para a pergunta personalizada e as propriedades da pergunta personalizada no momento da criação do compromisso.
author: razortbone
ms.localizationpriority: medium
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 1b62344b936c0c95b4e831c48c7b2d921c3033a0
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/15/2021
ms.locfileid: "61526475"
---
# <a name="bookingquestionanswer-resource-type"></a>Tipo de recurso bookingQuestionAnswer

Namespace: microsoft.graph

Contém uma pergunta personalizada, a resposta dada pelo cliente para a pergunta personalizada e as propriedades da pergunta personalizada no momento da criação do compromisso.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|answer|Cadeia de caracteres|A resposta dada pelo usuário no caso de **answerInputType** ser `text` .|
|answerInputType|answerInputType|O tipo de resposta esperado. Os valores possíveis são: `text`, `radioButton`, `unknownFutureValue`.|
|answerOptions|Coleção de cadeias de caracteres|No caso de **answerInputType** `radioButton` ser , isso consiste em uma lista de valores de resposta possíveis.|
|isRequired|Booliano|Indica se é obrigatório responder à pergunta personalizada.|
|question|Cadeia de caracteres|A pergunta.|
|questionId|Cadeia de caracteres|A ID da pergunta personalizada.|
|selectedOptions|Coleção de cadeias de caracteres|As respostas selecionadas pelo usuário.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.bookingQuestionAnswer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bookingQuestionAnswer",
  "questionId": "String",
  "question": "String",
  "answerInputType": {"@odata.type": "microsoft.graph.answerInputType"},
  "answerOptions": [
    "String"
  ],
  "isRequired": "Boolean",
  "answer": "String",
  "selectedOptions": [
    "String"
  ]
}
```

