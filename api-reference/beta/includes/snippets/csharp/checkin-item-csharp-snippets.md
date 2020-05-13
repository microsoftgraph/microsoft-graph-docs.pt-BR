---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7024a2bc21af591064697f77d5c1b5c67cb5e673
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2020
ms.locfileid: "37402142"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var comment = "Updating the latest guidelines";

await graphClient.Drives["{drive-id}"].Items["{item-id}"]
    .Checkin(null,comment)
    .Request()
    .PostAsync();

```