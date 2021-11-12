---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 257d2624c752a36bf32766a17ba7b41bda2747c9b60a5d09b052051d1874d267
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273716"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var type = "edit";

var scope = "organization";

await graphClient.Me.Drive.Items["{driveItem-id}"]
    .CreateLink(type,scope,null,null,null,null)
    .Request()
    .PostAsync();

```