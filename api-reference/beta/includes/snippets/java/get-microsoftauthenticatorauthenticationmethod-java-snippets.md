---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 13de7a1f7d41fbbd8237d2715919c3a1da24fe3e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50979694"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

MicrosoftAuthenticatorAuthenticationMethod microsoftAuthenticatorAuthenticationMethod = graphClient.users("anirban@contoso.com").authentication().microsoftAuthenticatorMethods("_jpuR-TGZtk6aQCLF3BQjA2")
    .buildRequest()
    .get();

```