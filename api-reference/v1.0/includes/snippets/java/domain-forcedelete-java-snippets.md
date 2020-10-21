---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 57a7d76afaf57fbdc1281eafbcbc9ea8a5c9d0ca
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48607591"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

boolean disableUserAccounts = true;

graphClient.domains("{id}")
    .forceDelete(disableUserAccounts)
    .buildRequest()
    .post();

```