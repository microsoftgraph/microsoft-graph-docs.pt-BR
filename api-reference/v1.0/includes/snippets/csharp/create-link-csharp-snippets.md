---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c6bcff99f8011c5fbb3da0b483b3c9ca9c97575e
ms.sourcegitcommit: df2c52f84aae5d4fed641d7411ba547371f0eaad
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2020
ms.locfileid: "44055605"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var type = "view";

var password = "ThisIsMyPrivatePassword";

var scope = "anonymous";

await graphClient.Me.Drive.Items["{item-id}"]
    .CreateLink(type,scope,null,password,null)
    .Request()
    .PostAsync();

```