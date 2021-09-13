---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2deb9fe18a5ff1a288af98fb29a055ca06fdc88a18060670e1bd3ef193ccd98f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56897766"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plans = await graphClient.Planner.Plans
    .Request()
    .GetAsync();

```