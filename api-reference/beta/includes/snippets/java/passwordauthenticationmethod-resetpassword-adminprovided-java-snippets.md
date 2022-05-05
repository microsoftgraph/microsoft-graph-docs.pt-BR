---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d6172a3ccdf4461b94af842226acec2389c5d253
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65220222"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String newPassword = "Cuyo5459";

graphClient.users("6ea91a8d-e32e-41a1-b7bd-d2d185eed0e0").authentication().passwordMethods("28c10230-6103-485e-b985-444c60001490")
    .resetPassword(AuthenticationMethodResetPasswordParameterSet
        .newBuilder()
        .withNewPassword(newPassword)
        .withRequireChangeOnNextSignIn(null)
        .build())
    .buildRequest()
    .post();

```