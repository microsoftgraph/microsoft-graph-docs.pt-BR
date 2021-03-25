---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c796b869545afb052a9b329191129ed3b34da693
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51202175"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WindowsHelloForBusinessAuthenticationMethod windowsHelloForBusinessAuthenticationMethod = graphClient.users("annie@contoso.com").authentication().windowsHelloForBusinessMethods("_jpuR-TGZtk6aQCLF3BQjA2")
    .buildRequest()
    .get();

```