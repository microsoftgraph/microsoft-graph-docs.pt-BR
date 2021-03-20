---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 55571705a99789f1469c76d1afd60211c06a725f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50978092"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TemporaryAccessPassAuthenticationMethod temporaryAccessPassAuthenticationMethod = new TemporaryAccessPassAuthenticationMethod();
temporaryAccessPassAuthenticationMethod.startDateTime = OffsetDateTimeSerializer.deserialize("2021-01-26T00:00:00Z");
temporaryAccessPassAuthenticationMethod.lifetimeInMinutes = 60;
temporaryAccessPassAuthenticationMethod.isUsableOnce = false;

graphClient.users("kim@contoso.com").authentication().temporaryAccessPassMethods()
    .buildRequest()
    .post(temporaryAccessPassAuthenticationMethod);

```