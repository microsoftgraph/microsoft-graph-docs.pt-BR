---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fb1fcc2d48aa7b2183b947e085c3c72c1e74ae63
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50978771"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String newPassword = "newPassword-value";

graphClient.users("{id | userPrincipalName}").authentication().passwordMethods("{id}")
    .resetPassword(AuthenticationMethodResetPasswordParameterSet
        .newBuilder()
        .withNewPassword(newPassword)
        .withRequireChangeOnNextSignIn(null)
        .build())
    .buildRequest()
    .post();

```