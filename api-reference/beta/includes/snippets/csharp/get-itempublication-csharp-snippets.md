---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1672434d9c5b7ccee7f9b6e3db2301f53754731e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800630"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var itemPublication = await graphClient.Me.Profile.Publications["{itemPublication-id}"]
    .Request()
    .GetAsync();

```