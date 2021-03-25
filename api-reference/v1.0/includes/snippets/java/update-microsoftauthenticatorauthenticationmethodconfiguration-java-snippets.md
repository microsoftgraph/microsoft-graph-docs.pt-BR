---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b6ac322747a16803151c597c207ab9cd4c14922d
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51202700"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

MicrosoftAuthenticatorAuthenticationMethodConfiguration authenticationMethodConfiguration = new MicrosoftAuthenticatorAuthenticationMethodConfiguration();
authenticationMethodConfiguration.state = AuthenticationMethodState.ENABLED;

graphClient.policies().authenticationMethodsPolicy().authenticationMethodConfigurations("microsoftAuthenticator")
    .buildRequest()
    .patch(authenticationMethodConfiguration);

```