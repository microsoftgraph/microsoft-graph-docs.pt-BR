---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0fdd77a80e7cdf6c4eb9c71d1944aafb1255df4defae0fdbec65753984536e3a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57275363"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AuthenticationFlowsPolicy authenticationFlowsPolicy = new AuthenticationFlowsPolicy();
SelfServiceSignUpAuthenticationFlowConfiguration selfServiceSignUp = new SelfServiceSignUpAuthenticationFlowConfiguration();
selfServiceSignUp.isEnabled = true;
authenticationFlowsPolicy.selfServiceSignUp = selfServiceSignUp;

graphClient.policies().authenticationFlowsPolicy()
    .buildRequest()
    .patch(authenticationFlowsPolicy);

```