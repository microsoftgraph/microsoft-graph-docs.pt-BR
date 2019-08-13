---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a107888fbc04500defd73a31de77e409a7eae228
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36359562"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getSharePointSiteUsageStorage = await graphClient.Reports
    .GetSharePointSiteUsageStorage("D7")
    .Request()
    .GetAsync();

```