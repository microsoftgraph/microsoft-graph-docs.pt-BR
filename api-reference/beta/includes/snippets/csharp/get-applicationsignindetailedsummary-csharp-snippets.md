---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fd805d0ef576f5df18cdc6502e66b16c108625e6d7007fd628b4b811d33b625e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56898926"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var applicationSignInDetailedSummary = await graphClient.Reports.ApplicationSignInDetailedSummary["{applicationSignInDetailedSummary-id}"]
    .Request()
    .GetAsync();

```