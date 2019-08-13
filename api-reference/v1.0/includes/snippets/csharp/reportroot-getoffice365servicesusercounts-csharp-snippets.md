---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 674630050d4891f10ec110bed4a6c9122df46671
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36374370"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetOffice365ServicesUserCounts("D7")
    .Request()
    .GetAsync();

```