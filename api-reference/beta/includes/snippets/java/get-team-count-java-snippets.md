---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8d4c7dbed3777ea31b622d54dd5149b2159809e1
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48979701"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("ConsistencyLevel", "eventual"));
requestOptions.add(new QueryOption("$search", "displayName:Team"));

IServicePrincipalCollectionPage servicePrincipals = graphClient.servicePrincipals()
    .buildRequest( requestOptions )
    .get();

```