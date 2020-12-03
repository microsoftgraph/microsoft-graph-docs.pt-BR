---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 61e02b9390c9f49297377bd90c418e86899b0118
ms.sourcegitcommit: d09d720b56ed6f1fad556e2a3730c2e850db355f
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/02/2020
ms.locfileid: "49556321"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

User user = new User();
user.accountEnabled = true;
user.displayName = "Adele Vance";
user.mailNickname = "AdeleV";
user.userPrincipalName = "AdeleV@contoso.onmicrosoft.com";
PasswordProfile passwordProfile = new PasswordProfile();
passwordProfile.forceChangePasswordNextSignIn = true;
passwordProfile.password = "xWwvJ]6NMw+bWH-d";
user.passwordProfile = passwordProfile;

graphClient.users()
    .buildRequest()
    .post(user);

```