---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 37f25e2108917efc07551064668853129bb9a63f
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36349354"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetSharePointSiteUsageStorage("D7")
    .Request()
    .GetAsync();

```