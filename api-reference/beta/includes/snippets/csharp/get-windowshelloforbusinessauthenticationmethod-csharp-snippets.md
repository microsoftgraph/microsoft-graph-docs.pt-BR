---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e5374f3a4c293347014fe9ff1f2f97618012cd2e
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444621"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var windowsHelloForBusinessAuthenticationMethod = await graphClient.Users["annie@contoso.com"].Authentication.WindowsHelloForBusinessMethods["_jpuR-TGZtk6aQCLF3BQjA2"]
    .Request()
    .GetAsync();

```