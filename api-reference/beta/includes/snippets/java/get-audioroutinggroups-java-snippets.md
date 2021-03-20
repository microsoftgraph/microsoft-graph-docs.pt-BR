---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3579e6a3f076b7d9cecf962d9114849791aaa1a3
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50977130"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AudioRoutingGroupCollectionPage audioRoutingGroups = graphClient.communications().calls("{id}").audioRoutingGroups()
    .buildRequest()
    .get();

```