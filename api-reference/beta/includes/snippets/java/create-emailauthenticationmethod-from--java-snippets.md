---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dabd45ccb8905ac93cc59e20d1994712592e3132
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2020
ms.locfileid: "49522486"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EmailAuthenticationMethod emailAuthenticationMethod = new EmailAuthenticationMethod();
emailAuthenticationMethod.emailAddress = "kim@contoso.com";

graphClient.users("kim@contoso.com").authentication().emailMethods()
    .buildRequest()
    .post(emailAuthenticationMethod);

```