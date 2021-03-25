---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 823fed860541130b40c383d0da3368eb0b04f4fa
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51202290"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Fido2AuthenticationMethodConfiguration authenticationMethodConfiguration = new Fido2AuthenticationMethodConfiguration();
authenticationMethodConfiguration.state = AuthenticationMethodState.ENABLED;
authenticationMethodConfiguration.isAttestationEnforced = false;

graphClient.policies().authenticationMethodsPolicy().authenticationMethodConfigurations("fido2")
    .buildRequest()
    .patch(authenticationMethodConfiguration);

```