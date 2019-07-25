---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ac2dd78f8333c87282af109137d5b1ea61b34015
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35869258"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("Authorization", "Bearer <token>"));

SynchronizationJobRestartCriteria criteria = new SynchronizationJobRestartCriteria();
criteria.resetScope = SynchronizationJobRestartScope.WATERMARK;

graphClient.servicePrincipals("{id}").synchronization().jobs("{jobId}")
    .restart(criteria)
    .buildRequest( requestOptions )
    .post();

```