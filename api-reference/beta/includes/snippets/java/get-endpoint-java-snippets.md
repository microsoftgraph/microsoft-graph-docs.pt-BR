---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: acb3e709bc4ada83ccee9f072bb076081e246c32
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48955051"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Endpoint endpoint = graphClient.groups("{id}").endpoints("{id}")
    .buildRequest()
    .get();

```