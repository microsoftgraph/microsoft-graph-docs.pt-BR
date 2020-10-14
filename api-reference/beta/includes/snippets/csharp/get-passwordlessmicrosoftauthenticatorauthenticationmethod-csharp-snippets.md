---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bfe6ee03c0a4336f2f52708cd572ea2384caa4a0
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/14/2020
ms.locfileid: "48457316"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var passwordlessMicrosoftAuthenticatorMethods = await graphClient.Me.Authentication.PasswordlessMicrosoftAuthenticatorMethods
    .Request()
    .GetAsync();

```