---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 71592caa2fef3ff005bd2e8f868fb2f09ceeb06d
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35869392"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SynchronizationJob synchronizationJob = graphClient.servicePrincipals("{id}").synchronization().jobs("{jobId}")
    .buildRequest()
    .get();

```