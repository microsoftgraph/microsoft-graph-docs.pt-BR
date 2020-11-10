---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5fb473197d8a5943107f8d4bd689018c6a02db07
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48955278"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IEducationUserDeltaCollectionPage delta = graphClient.education().users()
    .delta()
    .buildRequest()
    .get();

```