---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 081a7f1aface6ec00a2595ed00b55a5b8a39bc39ae8250c1b97dc71bd2d4ac6e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56897853"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ScreenSharingRole role = ScreenSharingRole.VIEWER;

graphClient.communications().calls("{id}")
    .changeScreenSharingRole(CallChangeScreenSharingRoleParameterSet
        .newBuilder()
        .withRole(role)
        .build())
    .buildRequest()
    .post();

```