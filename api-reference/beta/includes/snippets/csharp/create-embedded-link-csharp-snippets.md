---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 533411775a8b325a6b88f4efdade0feb7acfdb4d
ms.sourcegitcommit: 46ee19b244349e2a1537f0c44c576d7c01cf03a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/05/2019
ms.locfileid: "37402183"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var type = "embed";

await graphClient.Me.Drive.Items["{item-id}"]
    .CreateLink(type,null,null,null,null,null)
    .Request()
    .PostAsync();

```