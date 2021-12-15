---
title: Tipo de recurso bookingQuestionAssignment
description: Contém o conjunto de perguntas personalizadas associadas a um serviço específico.
ms.localizationpriority: medium
author: razortbone
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 8cab833de9bab5e07f72800e01816e437a747846
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/15/2021
ms.locfileid: "61525603"
---
# <a name="bookingquestionassignment-resource-type"></a>Tipo de recurso bookingQuestionAssignment

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contém o conjunto de perguntas personalizadas associadas a um serviço específico.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|isRequired|Booliano|Indica se é obrigatório responder à pergunta personalizada. |
|questionId|Cadeia de caracteres|Se for obrigatório responder à pergunta personalizada. |

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.bookingQuestionAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bookingQuestionAssignment",
  "questionId": "String",
  "isRequired": "Boolean"
}
```

