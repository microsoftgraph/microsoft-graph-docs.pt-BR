---
title: Tipo de recurso meetingRegistrant
description: Representa um registro de reunião que se registrou em uma reunião online.
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: dbc90ecc79258ad150077d474fcdd8d4b29f6db6
ms.sourcegitcommit: c3f849e5a052b1926373a4b316ec303250e6d09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/15/2021
ms.locfileid: "60369442"
---
# <a name="meetingregistrant-resource-type"></a>Tipo de recurso meetingRegistrant

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um registro de reunião que se registrou em uma [reunião online.](onlinemeeting.md)

## <a name="methods"></a>Métodos

| Método | Tipo de retorno | Descrição |
| :----- | :---------- | :---------- |
|[List](../api/meetingregistration-list-registrants.md) | [meetingRegistrant](meetingregistrant.md) | Listar todos os registrantes que se registraram na reunião. |
|[Criar](../api/meetingregistration-post-registrants.md) | [meetingRegistrant](meetingregistrant.md) | Registre um registro em uma reunião online. |
|[Excluir](../api/meetingregistrant-delete.md) | [meetingRegistrant](meetingregistrant.md) | Desinfete um registro de uma reunião online. |

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
| :------- | :--- | :---------- |
| customQuestionAnswers | [Coleção customQuestionAnswer](customQuestionAnswer.md) | A resposta do registro para perguntas personalizadas. |
| email | Cadeia de caracteres | O endereço de email do registrante. |
| firstName | Cadeia de caracteres | O primeiro nome do registro. |
| id | Cadeia de caracteres | A ID do registro. Apenas leitura. |
| joinWebUrl | Cadeia de caracteres | Uma URL da Web exclusiva para o registro ingressar na reunião. Apenas leitura. |
| lastName | Cadeia de caracteres | O sobrenome do registro. |
| registrationDateTime | Cadeia de caracteres | Hora em UTC quando o registrante se registrar na reunião. Somente leitura. |
| status | [meetingRegistrantStatus](#meetingregistrantstatus-values) | O status de registro do registrante. Apenas leitura. |

### <a name="meetingregistrantstatus-values"></a>valores meetingRegistrantStatus

| Valor              | Descrição |
|--------------------|-------------|
| registered | O Registrante se registrou na reunião. |
| cancelado | O Registro cancelou o registro. |
| processamento | Status provisório indicando que o status está sendo processado. |
| unknownFutureValue | Valor de sentinela de enumeração evolvável. Não usar. |

## <a name="json-representation"></a>Representação JSON

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.meetingRegistrant"
}-->

```json
{
  "id": "String",
  "firstName": "String (timestamp)",
  "email": "String",
  "lastName": "String",
  "joinWebUrl": "String",
  "registrationDateTime": "String (timestamp)",
  "status": { "@odata.type": "microsoft.graph.meetingRegistrantStatus" },
  "customQuestionAnswers": [{ "@odata.type": "microsoft.graph.customQuestionAnswer" }]
}
```
