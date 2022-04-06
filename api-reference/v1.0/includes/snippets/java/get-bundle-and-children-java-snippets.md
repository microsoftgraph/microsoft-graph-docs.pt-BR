---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 93e43d411fc302b335457d38700c9ac544190197
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2022
ms.locfileid: "63757956"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new QueryOption("expand", "children"));

DriveItem driveItem = graphClient.drive().items("{bundle-id}")
    .buildRequest( requestOptions )
    .get();

```