---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8110946a395de840f05191fca3153efd7a74340a
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50952950"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SynchronizationSchema synchronizationSchema = graphClient.servicePrincipals("{id}").synchronization().jobs("{jobId}").schema()
    .buildRequest()
    .get();

```