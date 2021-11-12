---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e4fe25279ad0f400f7b465d8301c8fd775c94ce496f2aec581c7c65a3cb349b3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102484"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plannerBucket = await graphClient.Planner.Buckets["{plannerBucket-id}"]
    .Request()
    .GetAsync();

```