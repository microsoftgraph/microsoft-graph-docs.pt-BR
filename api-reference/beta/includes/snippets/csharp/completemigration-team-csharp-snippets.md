---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ebba3b1955a8888b7f24e240682f91a449a76caf
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50783148"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Teams["{team-id}"]
    .CompleteMigration()
    .Request()
    .PostAsync();

```