---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 38fae9afcad3428d553db21fc2126fad53ef2bf7
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48977685"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

RiskDetection riskDetection = graphClient.identityProtection().riskDetections("c2b6c2b9-dddc-acd0-2b39-d519d803dbc3")
    .buildRequest()
    .get();

```