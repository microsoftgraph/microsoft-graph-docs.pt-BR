---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c5f4094996e593c46c91af99ac9a3cad91d03c7b
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51210615"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ChatMessageDeltaCollectionPage delta = graphClient.teams("{id}").channels("{id}").messages()
    .delta()
    .buildRequest()
    .skipToken("c3RhcnRUaW1lPTE1NTEyODcyMzY2NzgmcGFnZVNpemU9MjA=")
    .get();

```