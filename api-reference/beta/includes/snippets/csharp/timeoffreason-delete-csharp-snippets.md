---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4660922f8ef5e4fb59ca3f689a1b9c53eff6f973d3c1bf3d5015a7b90f981539
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100335"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Teams["{team-id}"].Schedule.TimeOffReasons["{timeOffReason-id}"]
    .Request()
    .DeleteAsync();

```