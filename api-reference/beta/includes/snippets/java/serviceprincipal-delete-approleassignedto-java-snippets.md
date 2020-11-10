---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 861fdc1ab18fff14eb5a9a2e80f4fc2efb6225d5
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48970804"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.servicePrincipals("{id}").appRoleAssignedTo("{id}")
    .buildRequest()
    .delete();

```