---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c2632754f847180622a45953fb9ca68dbfbfc686
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48970440"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrivilegedRole privilegedRole = graphClient.privilegedRoles("{id}")
    .buildRequest()
    .get();

```