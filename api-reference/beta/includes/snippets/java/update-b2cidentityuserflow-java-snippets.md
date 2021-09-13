---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e653e548a4fc22bbbb78f94305a107fef61bc6d3ca3b4a396e7295fdae592655
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157441"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

B2cIdentityUserFlow b2cIdentityUserFlow = new B2cIdentityUserFlow();
b2cIdentityUserFlow.isLanguageCustomizationEnabled = true;
b2cIdentityUserFlow.defaultLanguageTag = "en";

graphClient.identity().b2cUserFlows("B2C_1_CustomerSignUp")
    .buildRequest()
    .patch(b2cIdentityUserFlow);

```