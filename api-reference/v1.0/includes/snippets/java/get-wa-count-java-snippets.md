---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 856a4a2a269248beed2ea43c0399842badf95d6c
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59764402"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("ConsistencyLevel", "eventual"));
requestOptions.add(new QueryOption("$search", "displayName:wa"));

UserCollectionPage users = graphClient.users()
    .buildRequest( requestOptions )
    .orderBy("displayName")
    .get();

```