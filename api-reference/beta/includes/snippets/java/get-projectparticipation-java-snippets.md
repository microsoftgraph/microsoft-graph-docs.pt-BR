---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dc3ce189d862d806398d83a61949c062e113266c
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48980017"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ProjectParticipation projectParticipation = graphClient.me().profile().projects("{id}")
    .buildRequest()
    .get();

```