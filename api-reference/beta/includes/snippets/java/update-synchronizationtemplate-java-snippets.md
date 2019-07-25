---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8919ba5b11107aa73918851fac69dc8e344a9257
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35869030"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("Authorization", "Bearer <token>"));

SynchronizationTemplate synchronizationTemplate = new SynchronizationTemplate();
synchronizationTemplate.id = "Slack";
synchronizationTemplate.applicationId = "{id}";
synchronizationTemplate.factoryTag = "CustomSCIM";

graphClient.applications("{id}").synchronization().templates("{templateId}")
    .buildRequest( requestOptions )
    .put(synchronizationTemplate);

```