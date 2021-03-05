---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 702d84e349b74998366c06599aa7aee8b7c6dd30
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50475294"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Policies.AuthenticationMethodsPolicy.AuthenticationMethodConfigurations["microsoftAuthenticator"]
    .Request()
    .DeleteAsync();

```