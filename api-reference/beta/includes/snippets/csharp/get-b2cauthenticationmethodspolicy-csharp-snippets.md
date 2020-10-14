---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dc72595fa873bec111b17de38a49196ab196af34
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/14/2020
ms.locfileid: "48457336"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var b2cAuthenticationMethodsPolicy = await graphClient.Policies.B2cAuthenticationMethodsPolicy
    .Request()
    .GetAsync();

```