---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7eafaa43a73513acd6f2348c36b6d1b9403c6f37d21adb82ab40c4fc88752374
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899067"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var riskyUserHistoryItem = await graphClient.RiskyUsers["{riskyUser-id}"].History["{riskyUserHistoryItem-id}"]
    .Request()
    .GetAsync();

```