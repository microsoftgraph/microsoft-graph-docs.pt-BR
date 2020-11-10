---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 84c5cbceae977e826c4faa3140a1db142fadf061
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48969635"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.servicePrincipals("{id}")
    .buildRequest()
    .delete();

```