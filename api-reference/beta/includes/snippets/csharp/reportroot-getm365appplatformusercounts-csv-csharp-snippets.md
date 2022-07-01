---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 25eca666e19647f4d8eafc7d9b6704ee40d7a26d
ms.sourcegitcommit: af9489bd42a25dff04836dcfcc57369259fda587
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2022
ms.locfileid: "66577915"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var stream = await graphClient.Reports
    .GetM365AppPlatformUserCounts("D7")
    .Request()
    .GetAsync();

```