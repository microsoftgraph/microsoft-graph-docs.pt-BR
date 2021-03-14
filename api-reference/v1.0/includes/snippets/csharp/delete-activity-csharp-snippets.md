---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 78e4602eed7e0f617a7ef32f3e80ee87ef3286a0
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50799775"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Activities["{userActivity-id}"]
    .Request()
    .DeleteAsync();

```