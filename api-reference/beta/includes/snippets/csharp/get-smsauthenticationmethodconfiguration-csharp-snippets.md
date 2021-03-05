---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1881bdef13af0da42b214ba5055fdbf5c5f1ee93
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50475591"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var authenticationMethodConfiguration = await graphClient.Policies.AuthenticationMethodsPolicy.AuthenticationMethodConfigurations["sms"]
    .Request()
    .GetAsync();

```