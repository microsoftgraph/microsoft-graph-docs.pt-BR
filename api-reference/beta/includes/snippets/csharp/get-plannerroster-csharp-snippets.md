---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: de937f5788f80bd2db4d28a16454a1a597cc247e0ccc46795ea75b0dd8a23e10
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214741"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plannerRoster = await graphClient.Planner.Rosters["{plannerRoster-id}"]
    .Request()
    .GetAsync();

```