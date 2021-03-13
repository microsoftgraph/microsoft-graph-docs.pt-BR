---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: da387d740f561edf309d316d37e6ad9a6c1c474a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50789256"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var subscription = await graphClient.Me.Drive.Root.Subscriptions["{subscription-id}"]
    .Request()
    .GetAsync();

```