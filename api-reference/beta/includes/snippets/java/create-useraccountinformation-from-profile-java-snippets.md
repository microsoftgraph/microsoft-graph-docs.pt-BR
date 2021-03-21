---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 07d3bc970df93aac3745c49bd9f50d31da31bee4
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50978793"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserAccountInformation userAccountInformation = new UserAccountInformation();
userAccountInformation.allowedAudiences = EnumSet.of(AllowedAudiences.ORGANIZATION);
userAccountInformation.countryCode = "NO";

graphClient.me().profile().account()
    .buildRequest()
    .post(userAccountInformation);

```