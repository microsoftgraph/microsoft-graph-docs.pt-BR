---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ff65b78827bf251d317f31ea9b854d740911e44dac982831f9bfe18f275a052b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272539"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tasks = await graphClient.Planner.Buckets["{plannerBucket-id}"].Tasks
    .Request()
    .GetAsync();

```