---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cc66b30c80510ddce0e774e371c910c82a3c107f
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48980227"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TokenLifetimePolicy tokenLifetimePolicy = graphClient.policies().tokenLifetimePolicies("{id}")
    .buildRequest()
    .get();

```