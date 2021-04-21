---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ffdc14570ba6ba5098f5c0918deb81701fbe41bd
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921453"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityProviderBase identityProviderBase = graphClient.identity().identityProviders("OIDC-V1-test-icm-4470de58-86c2-4a3f-a22c-63c9366cd000")
    .buildRequest()
    .get();

```