---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cc5534413efc4eb423a070e89013a8199bd4a7d6
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53209386"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("ConsistencyLevel", "eventual"));

UserCollectionPage user = graphClient.groups("{id}").transitiveMembers().microsoft.graph.user()
    .buildRequest( requestOptions )
    .filter("startswith(displayName, 'a')")
    .orderBy("displayName")
    .get();

```