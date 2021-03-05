---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1170690a3b3d7de5299c61a7faca90a427802048
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50472951"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Policies.AuthenticationMethodsPolicy.AuthenticationMethodConfigurations["email"]
    .Request()
    .DeleteAsync();

```