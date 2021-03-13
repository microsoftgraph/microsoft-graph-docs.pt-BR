---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a983dc370c36a2dd4df298f9ec69b39a42e47751
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50802028"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var stream = await graphClient.Me.Onenote.Resources["{onenoteResource-id}"].Content
    .Request()
    .GetAsync();

```