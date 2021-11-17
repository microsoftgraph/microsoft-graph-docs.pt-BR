---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a4864830da3f6e7f62d86022d9c5c66533d0b9cd
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61030805"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityProviderBase identityProviderBase = new IdentityProviderBase();
identityProviderBase.displayName = "Apple";

graphClient.identity().identityProviders("Apple-Managed-OIDC")
    .buildRequest()
    .patch(identityProviderBase);

```