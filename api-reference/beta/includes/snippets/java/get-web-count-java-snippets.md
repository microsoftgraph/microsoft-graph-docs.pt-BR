---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 05ef46aa2ea11990819352af33fc62cd4bb2cd55
ms.sourcegitcommit: 5bb981b4853663354a566d4a4a5cbf288939e441
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/24/2021
ms.locfileid: "53579343"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("ConsistencyLevel", "eventual"));
requestOptions.add(new QueryOption("$search", "displayName:Web"));

ApplicationCollectionPage applications = graphClient.applications()
    .buildRequest( requestOptions )
    .get();

```