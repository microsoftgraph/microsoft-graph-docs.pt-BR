---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 462e307d248212475fb7f268db04bf96e6701eb4
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35498244"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getSharePointActivityPages = await graphClient.Reports.GetSharePointActivityPages('D7')
    .Request()
    .GetAsync();

```