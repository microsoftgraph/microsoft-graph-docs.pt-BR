---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: edf12b87e316ce09d95a6f76b23059995231605b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50969432"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityUserFlowCollectionPage userFlows = graphClient.identity().userFlows()
    .buildRequest()
    .get();

```