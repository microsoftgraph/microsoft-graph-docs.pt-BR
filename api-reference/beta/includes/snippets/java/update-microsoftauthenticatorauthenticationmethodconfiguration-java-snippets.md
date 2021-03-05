---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b69affbc193a70e9831f233c4c192baa980d5924
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50473008"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

MicrosoftAuthenticatorAuthenticationMethodConfiguration authenticationMethodConfiguration = new MicrosoftAuthenticatorAuthenticationMethodConfiguration();
authenticationMethodConfiguration.state = AuthenticationMethodState.ENABLED;

graphClient.policies().authenticationMethodsPolicy().authenticationMethodConfigurations("microsoftAuthenticator")
    .buildRequest()
    .patch(authenticationMethodConfiguration);

```