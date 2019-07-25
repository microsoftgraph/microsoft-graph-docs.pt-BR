---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6bc74d9cf0f198f11fd03f5528b6977ff523e519
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35869417"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Subscription subscription = new Subscription();
subscription.expirationDateTime = "2016-11-22T18:23:45.9356913Z";

graphClient.subscriptions("{id}")
    .buildRequest()
    .patch(subscription);

```