---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2b0a614aecef270a2a407c997ebe3fe9f499ebe313661efe4ef80befc22d01f5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102571"
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