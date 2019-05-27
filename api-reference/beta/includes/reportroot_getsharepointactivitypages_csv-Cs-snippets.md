---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 462e307d248212475fb7f268db04bf96e6701eb4
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34440790"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getSharePointActivityPages = await graphClient.Reports.GetSharePointActivityPages('D7')
    .Request()
    .GetAsync();

```