---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6461b7d1a76e90383622f43f7d821f2eef91869c8f98b375de91a06cb58431b0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899072"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var history = await graphClient.IdentityProtection.RiskyUsers["{riskyUser-id}"].History
    .Request()
    .GetAsync();

```