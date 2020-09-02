---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e491d30b1bc48dc511c819702a41838b305baa80
ms.sourcegitcommit: 726f20403323be7d267b67c2764ed7c244e02ee1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/02/2020
ms.locfileid: "47331085"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var search = await graphClient.Me.Drive.Root
    .Search("Contoso Project")
    .Request()
    .GetAsync();

```