---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dc0a163606ecdeedf2fb4c3a1c15029fe3713853
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48951484"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.teams("{teamId}")
    .completeMigration()
    .buildRequest()
    .post();

```