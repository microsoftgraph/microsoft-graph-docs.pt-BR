---
title: tipo de recurso meetingRegistrationQuestion
description: Representa uma pergunta de registro personalizada, diferente do nome, sobrenome e endereço de email, associada a uma meetingRegistration.
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 42645be07a3540294906cb03fb7b28c080bbd0ed
ms.sourcegitcommit: c3f849e5a052b1926373a4b316ec303250e6d09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/15/2021
ms.locfileid: "60370321"
---
# <a name="meetingregistrationquestion-resource-type"></a>tipo de recurso meetingRegistrationQuestion

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma pergunta de registro personalizada, diferente do nome, sobrenome e endereço de email, associada a [uma meetingRegistration](meetingRegistration.md).

## <a name="methods"></a>Métodos

| Método | Tipo de retorno | Descrição |
| :----- | :---------- | :---------- |
|[List](../api/meetingregistration-list-customquestions.md) | [coleção meetingRegistrationQuestion](meetingregistrationquestion.md) | Listar todas as perguntas de registro personalizadas. |
|[Criar](../api/meetingregistration-post-customquestions.md) | [meetingRegistrationQuestion](meetingregistrationquestion.md) | Crie uma pergunta de registro personalizada. |
|[Obter](../api/meetingregistrationquestion-get.md) | [meetingRegistrationQuestion](meetingregistrationquestion.md) | Obter uma pergunta de registro personalizada. |
|[Atualizar](../api/meetingregistrationquestion-update.md) | [meetingRegistrationQuestion](meetingregistrationquestion.md) | Atualize uma pergunta de registro personalizada. |
|[Excluir](../api/meetingregistrationquestion-delete.md) | [meetingRegistrationQuestion](meetingregistrationquestion.md) | Excluir uma pergunta de registro personalizada. |

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
| :------- | :--- | :---------- |
| answerInputType | [answerInputType](#answerinputtype-values) | Tipo de entrada de resposta da pergunta de registro personalizado. |
| answerOptions | String collection | Opções de resposta **quando answerInputType** é `radioButton` . |
| displayName | Cadeia de caracteres | Nome de exibição da pergunta de registro personalizado. |
| id | Cadeia de caracteres | ID da pergunta de registro personalizado. Apenas leitura. |
| isRequired | Booliano | Indica se a pergunta é necessária. O valor padrão é `false`. |

### <a name="answerinputtype-values"></a>valores answerInputType

| Valor              | Descrição |
|--------------------|-------------|
| texto | Question aceita uma única resposta de texto de linha. |
| radioButton | A pergunta aceita uma resposta escolhida de botões de rádio. |
| unknownFutureValue | Valor de sentinela de enumeração evolvável. Não usar. |

## <a name="json-representation"></a>Representação JSON

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.meetingRegistrationQuestion"
}-->

```json
{
  "id": "String",
  "displayName": "String",
  "isRequired": "Boolean",
  "answerInputType": { "@odata.type": "microsoft.graph.answerInputType" },
  "answerOptions": [ "String" ],
}
```
