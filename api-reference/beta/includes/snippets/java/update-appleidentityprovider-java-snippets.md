---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a4864830da3f6e7f62d86022d9c5c66533d0b9cd
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921212"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityProviderBase identityProviderBase = new IdentityProviderBase();
identityProviderBase.displayName = "Apple";

graphClient.identity().identityProviders("Apple-Managed-OIDC")
    .buildRequest()
    .patch(identityProviderBase);

```