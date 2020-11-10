---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 35a28ae0caaa32f2f4774c7f02a1cbefed7c3160
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48963154"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.servicePrincipals("{id}").synchronization().jobs("{jobId}").schema().directories("{directoryId}")
    .discover()
    .buildRequest()
    .post();

```