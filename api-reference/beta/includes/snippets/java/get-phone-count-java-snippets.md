---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8104b62d3b557879109af14080e6d63eee389622
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48972923"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("ConsistencyLevel", "eventual"));
requestOptions.add(new QueryOption("$search", "displayName:wa"));

IOrgContactCollectionPage contacts = graphClient.contacts()
    .buildRequest( requestOptions )
    .get();

```