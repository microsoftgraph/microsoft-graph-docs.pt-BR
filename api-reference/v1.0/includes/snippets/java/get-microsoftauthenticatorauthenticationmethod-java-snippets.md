---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 13de7a1f7d41fbbd8237d2715919c3a1da24fe3e
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51202794"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

MicrosoftAuthenticatorAuthenticationMethod microsoftAuthenticatorAuthenticationMethod = graphClient.users("anirban@contoso.com").authentication().microsoftAuthenticatorMethods("_jpuR-TGZtk6aQCLF3BQjA2")
    .buildRequest()
    .get();

```