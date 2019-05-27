---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 94fcf705ef40e5070a8efcdee82e99b4d0b1c680
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34459804"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{item-id}"]
    .Request()
    .DeleteAsync();

```