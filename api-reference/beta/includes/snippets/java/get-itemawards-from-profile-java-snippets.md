---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 67f40731121732614345a1966cc05d24bf9559f1
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48980801"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IPersonAwardCollectionPage awards = graphClient.me().profile().awards()
    .buildRequest()
    .get();

```