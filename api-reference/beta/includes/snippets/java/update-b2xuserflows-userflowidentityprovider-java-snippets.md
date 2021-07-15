---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b804b5c09ba187adbddbbe6851d32568e6d5b9e6
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439529"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityProviderBase userFlowIdentityProviders = new IdentityProviderBase();
userFlowIdentityProviders.additionalDataManager().put("@odata.id", new JsonPrimitive("https://graph.microsoft.com/beta/identity/identityProviders/B2X_1_Test"));

graphClient.identity().b2xUserFlows("B2X_1_Test").userFlowIdentityProviders().references()
    .buildRequest()
    .patch(userFlowIdentityProviders);

```