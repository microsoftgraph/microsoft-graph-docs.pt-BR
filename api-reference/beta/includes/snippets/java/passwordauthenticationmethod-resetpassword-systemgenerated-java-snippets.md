---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3f10d67c9fe658e401c24ae7227cf280729efa8bf24875f3a1d32bc13f716fe5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57160321"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.users("{id | userPrincipalName}").authentication().passwordMethods("{id}")
    .resetPassword(AuthenticationMethodResetPasswordParameterSet
        .newBuilder()
        .withNewPassword(null)
        .withRequireChangeOnNextSignIn(null)
        .build())
    .buildRequest()
    .post();

```