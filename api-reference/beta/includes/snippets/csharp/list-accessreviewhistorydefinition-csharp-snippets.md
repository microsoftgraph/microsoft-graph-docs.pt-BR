---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 78e18572e6d5ac306ea81b115e654653d28e0146373e44209036bd5b310a5252
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57156556"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var historyDefinitions = await graphClient.IdentityGovernance.AccessReviews.HistoryDefinitions
    .Request()
    .GetAsync();

```