---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4586fc819e26253a821a01efca42a7c74a9aabb9
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50778134"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Teams["{team-id}"]
    .Archive(null)
    .Request()
    .PostAsync();

```