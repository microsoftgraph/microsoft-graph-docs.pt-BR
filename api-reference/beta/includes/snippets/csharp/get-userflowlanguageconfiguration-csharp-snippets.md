---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c8339d32cb03886606bda2cf840a397010e5d424
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50809745"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var languages = await graphClient.Identity.B2cUserFlows["{b2cIdentityUserFlow-id}"].Languages
    .Request()
    .GetAsync();

```