---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 83d2c0eff5272bb04985f1c864598fbe16371704
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48967499"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IPrintUserIdentityCollectionPage allowedUsers = graphClient.print().shares("{id}").allowedUsers()
    .buildRequest()
    .get();

```