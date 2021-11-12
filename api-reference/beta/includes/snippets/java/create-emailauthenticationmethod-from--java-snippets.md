---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 493256df33c7d6832e587f35a2fd6e98967a8e2df2b15cc95805fe4d41e84877
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57271965"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EmailAuthenticationMethod emailAuthenticationMethod = new EmailAuthenticationMethod();
emailAuthenticationMethod.emailAddress = "kim@contoso.com";

graphClient.users("kim@contoso.com").authentication().emailMethods()
    .buildRequest()
    .post(emailAuthenticationMethod);

```