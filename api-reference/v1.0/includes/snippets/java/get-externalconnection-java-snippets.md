---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f743ac0829365d553b2e2604d208f2e2920e71ba
ms.sourcegitcommit: 5bb981b4853663354a566d4a4a5cbf288939e441
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/24/2021
ms.locfileid: "53580015"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ExternalConnection externalConnection = graphClient.connections("contosohr")
    .buildRequest()
    .get();

```