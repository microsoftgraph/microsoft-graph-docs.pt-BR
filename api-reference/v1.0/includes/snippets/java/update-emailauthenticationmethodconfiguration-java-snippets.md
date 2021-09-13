---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: eaf9daabb2a74cfbd2e9fb8e694a46bdf75fdf0989e0a3c1a02ff9534a1d9595
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899325"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EmailAuthenticationMethodConfiguration authenticationMethodConfiguration = new EmailAuthenticationMethodConfiguration();
authenticationMethodConfiguration.allowExternalIdToUseEmailOtp = ExternalEmailOtpState.ENABLED;

graphClient.policies().authenticationMethodsPolicy().authenticationMethodConfigurations("email")
    .buildRequest()
    .patch(authenticationMethodConfiguration);

```