---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 79f55fdfb530f3c43d8fe2abf0d3beb50fa2eb55
ms.sourcegitcommit: af9489bd42a25dff04836dcfcc57369259fda587
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2022
ms.locfileid: "66577904"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var stream = await graphClient.Reports
    .GetM365AppUserCounts("D7")
    .Request()
    .GetAsync();

```