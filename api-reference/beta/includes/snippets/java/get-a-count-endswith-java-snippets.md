---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: de6b5ab57daba65fd6ee31e5483aa553d4189fde
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/27/2021
ms.locfileid: "50013406"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("ConsistencyLevel", "eventual"));

IUserCollectionPage users = graphClient.users()
    .buildRequest( requestOptions )
    .filter("endswith(mail,'a@contoso.com'),")
    .orderBy("userPrincipalName ")
    .get();

```