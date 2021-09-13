---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8de331effac8b0a4a74c9794267d2b19268ef5718999ea1e3754c69d8fe5e201
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899505"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tasks = await graphClient.Planner.Plans["{plannerPlan-id}"].Tasks
    .Request()
    .GetAsync();

```