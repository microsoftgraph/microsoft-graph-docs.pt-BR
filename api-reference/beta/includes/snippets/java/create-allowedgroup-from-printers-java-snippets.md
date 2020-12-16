---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c462c596b0d25e96867e0d4f9a9078faca4eefd3
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/16/2020
ms.locfileid: "49692797"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Group group = new Group();
group.additionalDataManager().put("@odata.id", new JsonPrimitive("https://graph.microsoft.com/beta/groups/{id}"));

graphClient.print().shares("{id}").allowedGroups().references()
    .buildRequest()
    .post(group);

```