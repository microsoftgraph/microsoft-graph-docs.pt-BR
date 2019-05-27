---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 25765918e83ccb7c3520364a2213f451eadf6edd
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34453618"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Directory.DeletedItems["46cc6179-19d0-473e-97ad-6ff84347bbbb"]
    .Restore()
    .Request()
    .PostAsync();

```