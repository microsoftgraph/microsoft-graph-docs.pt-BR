---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 73828376ed9cfc6d4f61257019fb8418b6d0486d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50798256"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groupLifecyclePolicies = await graphClient.Groups["{group-id}"].GroupLifecyclePolicies
    .Request()
    .GetAsync();

```