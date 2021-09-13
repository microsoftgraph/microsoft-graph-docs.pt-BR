---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fc92e7aad15f251f12e384221536a06b12e7789c7e1d3a7238be4b405ea578fc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57217076"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Groups["{group-id}"]
    .ResetUnseenCount()
    .Request()
    .PostAsync();

```