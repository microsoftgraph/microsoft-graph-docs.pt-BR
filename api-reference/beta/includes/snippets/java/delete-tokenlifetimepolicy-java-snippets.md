---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e84da1013766484f0a1568a9620e94790ec3421f
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48980246"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.policies().tokenLifetimePolicies("{id}")
    .buildRequest()
    .delete();

```