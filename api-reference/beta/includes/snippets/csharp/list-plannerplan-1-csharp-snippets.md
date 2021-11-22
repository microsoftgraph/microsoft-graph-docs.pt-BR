---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d199dba2e6b2a09a6e7be7486f6633ebcd1a715e744e0b2f489e15d17cadd78c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57271918"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plans = await graphClient.Planner.Rosters["{plannerRoster-id}"].Plans
    .Request()
    .GetAsync();

```