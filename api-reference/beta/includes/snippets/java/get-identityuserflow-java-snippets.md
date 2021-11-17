---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9adfcec577dee9ea68049ef5a9dd20217005a11d4bb7822070bd89e542273e70
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214765"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityUserFlow identityUserFlow = graphClient.identity().userFlows("B2C_1_Pol1")
    .buildRequest()
    .get();

```