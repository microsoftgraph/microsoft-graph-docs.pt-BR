---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2567fe583467afcd4b8bddd133e034078ce2ec90561c6ed1b3233525a8096c58
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57213963"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SynchronizationJob synchronizationJob = graphClient.servicePrincipals("{id}").synchronization().jobs("{jobId}")
    .buildRequest()
    .get();

```