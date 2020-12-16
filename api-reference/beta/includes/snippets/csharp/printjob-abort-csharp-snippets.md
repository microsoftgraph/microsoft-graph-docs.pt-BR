---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 94918c3273206613ffe38207852d8c7b6421a326
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/16/2020
ms.locfileid: "49691038"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Print.Printers["{id}"].Jobs["{id}"]
    .Abort(null)
    .Request()
    .PostAsync();

```