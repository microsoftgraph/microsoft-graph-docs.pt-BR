---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 76cb1411e08472adc5b8bbb2bf2a031d9c0db706
ms.sourcegitcommit: 9edfcf99706c8490cd5832a1c706a88a89e24db1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/07/2020
ms.locfileid: "42947546"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Print.Printers["{id}"].Jobs["{id}"]
    .CancelPrintJob()
    .Request()
    .PostAsync();

```