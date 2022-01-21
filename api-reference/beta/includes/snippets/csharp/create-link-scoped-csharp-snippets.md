---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c6bfd4ccf544dba9d1a96c52cd61ed9936a09e23
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62137598"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var type = "edit";

var scope = "organization";

await graphClient.Me.Drive.Items["{driveItem-id}"]
    .CreateLink(type,scope,null,null,null,null,null)
    .Request()
    .PostAsync();

```