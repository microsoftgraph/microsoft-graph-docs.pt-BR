---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 349379393407607c9637e8da818c3061738c6ccd
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50967655"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new QueryOption("filter", "bundle/album ne null"));

DriveItemCollectionPage bundles = graphClient.drive().bundles()
    .buildRequest( requestOptions )
    .filter("bundle/album ne null")
    .get();

```