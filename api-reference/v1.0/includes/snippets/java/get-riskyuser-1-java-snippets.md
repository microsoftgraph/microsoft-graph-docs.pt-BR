---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3cd6c4b0c06ebbd4202784ed3eb99b171cdae17b
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62132122"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

RiskyUser riskyUser = graphClient.identityProtection().riskyUsers("c2b6c2b9-dddc-acd0-2b39-d519d803dbc3")
    .buildRequest()
    .get();

```