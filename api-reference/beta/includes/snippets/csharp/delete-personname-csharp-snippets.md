---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fdd56fa40251e4dbdd79d10e761c5dc71e3b1926
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50782167"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Profile.Names["{personName-id}"]
    .Request()
    .DeleteAsync();

```