---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1166a18d5d24dfeb99852359b20f2a44039788ed6ce160c83171c54128d96e39
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899858"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Messages["{message-id}"].Extensions["{extension-id}"]
    .Request()
    .DeleteAsync();

```