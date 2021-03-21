---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 668a0eab6e980ec4bb28c1900b54a1560400159f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50977388"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

RoomListCollectionPage roomlist = graphClient.places().microsoft.graph.roomlist()
    .buildRequest()
    .get();

```