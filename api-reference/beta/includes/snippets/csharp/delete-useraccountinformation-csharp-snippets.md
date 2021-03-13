---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f8b6fffcf7d117caf7acba5b63ce9a13d4f45558
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50793218"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Profile.Account["{userAccountInformation-id}"]
    .Request()
    .DeleteAsync();

```