---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 40c6d90dc9e2d10efce99def34cdff4a570e2d53
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/14/2020
ms.locfileid: "48457520"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Users["kim@contoso.com"].Authentication.PasswordlessMicrosoftAuthenticatorMethods["R18B3t8Ogh9XIOGmPt81d6p_KXJs1YTxfGgGqeVFJSM1"]
    .Request()
    .DeleteAsync();

```