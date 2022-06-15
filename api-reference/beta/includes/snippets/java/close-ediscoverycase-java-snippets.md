---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f41042674f37b9f2c70046a25025b39b5f61b34f
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2022
ms.locfileid: "66095454"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.security().cases().ediscoveryCases("061b9a92-8926-4bd9-b41d-abf35edc7583")
    .close()
    .buildRequest()
    .post();

```