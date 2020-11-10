---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cfad6c05f932b8fd281e94026b844d45a8c318a3
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48971407"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ISynchronizationSchemaFunctionsCollectionPage functions = graphClient.servicePrincipals("{id}").synchronization().jobs("{jobId}").schema()
    .functions()
    .buildRequest()
    .get();

```