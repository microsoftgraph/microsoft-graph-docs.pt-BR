---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b18a1c5216a919e2756be05f81e0183cf6f01ee66d8804a7ec78c773c58e8404
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214324"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plannerBucketTaskBoardTaskFormat = await graphClient.Planner.Tasks["{plannerTask-id}"].BucketTaskBoardFormat
    .Request()
    .GetAsync();

```