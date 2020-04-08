---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a81417d4824a96ebfac2d3592abf74ac0ab7b5cb
ms.sourcegitcommit: 9edfcf99706c8490cd5832a1c706a88a89e24db1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/07/2020
ms.locfileid: "42948281"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printerShares = await graphClient.Print.PrinterShares
    .Request()
    .GetAsync();

```