---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a7a89616b566cd717dae05649d0d99cd60426da3
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50475619"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Policies.AuthenticationMethodsPolicy.AuthenticationMethodConfigurations["sms"]
    .Request()
    .DeleteAsync();

```