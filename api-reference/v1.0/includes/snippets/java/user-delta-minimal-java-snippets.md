---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 14f07e6544ea5ddc068010b731c7deaa8073b722
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50979454"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("Prefer", "return=minimal"));

UserDeltaCollectionPage delta = graphClient.users()
    .delta()
    .buildRequest( requestOptions )
    .select("displayName,jobTitle,mobilePhone")
    .get();

```