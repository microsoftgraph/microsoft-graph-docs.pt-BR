---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 491ad4b4f40ad9e4ed79bba7dd1565726a19252e
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/30/2020
ms.locfileid: "48315512"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Teams["{teamsId}"].Members["{membership-id}"]
    .Request()
    .DeleteAsync();

```