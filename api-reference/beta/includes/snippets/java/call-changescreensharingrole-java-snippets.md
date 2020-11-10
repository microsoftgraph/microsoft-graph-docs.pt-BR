---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 18a9b1396c5f0d3aea0025d2d995171c9f14f63b
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48959771"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ScreenSharingRole role = ScreenSharingRole.VIEWER;

graphClient.communications().calls("{id}")
    .changeScreenSharingRole(role)
    .buildRequest()
    .post();

```