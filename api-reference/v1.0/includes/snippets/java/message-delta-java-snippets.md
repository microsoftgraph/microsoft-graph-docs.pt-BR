---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 15125057a61aa5385fc96558108d40535bbc4e29
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50976265"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("Prefer", "odata.maxpagesize=2"));

MessageDeltaCollectionPage delta = graphClient.me().mailFolders("{id}").messages()
    .delta()
    .buildRequest( requestOptions )
    .get();

```