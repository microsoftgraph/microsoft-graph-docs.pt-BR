---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ef2ba1952a995b1a1cff5884761ae7def589cb42
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50982616"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new QueryOption("token", "latest"));

DriveItemDeltaCollectionPage delta = graphClient.me().drive().root()
    .delta()
    .buildRequest( requestOptions )
    .get();

```