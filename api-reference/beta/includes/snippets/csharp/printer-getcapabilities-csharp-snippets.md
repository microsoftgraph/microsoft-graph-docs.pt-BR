---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f74009ad464eba92e55c4bc1297ace5652c556c5
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447674"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printerCapabilities = await graphClient.Print.Printers["{id}"]
    .GetCapabilities()
    .Request()
    .GetAsync();

```