---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f27a750575b1e2220ee9cfcc19421c2621e2c226a831ea94a079af633de33cd7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157596"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plannerTaskDetails = await graphClient.Planner.Tasks["{plannerTask-id}"].Details
    .Request()
    .GetAsync();

```