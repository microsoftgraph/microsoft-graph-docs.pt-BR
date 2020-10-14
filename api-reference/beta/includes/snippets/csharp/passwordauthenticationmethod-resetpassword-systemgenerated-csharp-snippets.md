---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 38ac08e5e9661a66909ea6af563b336b80f8c6f3
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/14/2020
ms.locfileid: "48457553"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Users["{id | userPrincipalName}"].Authentication.PasswordMethods["{id}"]
    .ResetPassword(null,null)
    .Request()
    .PostAsync();

```