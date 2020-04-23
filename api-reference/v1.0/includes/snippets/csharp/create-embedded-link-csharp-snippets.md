---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 28a805fc4a3282bd78ba68c50fbd6791f56a6fce
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43771061"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var type = "embed";

await graphClient.Me.Drive.Items["{item-id}"]
    .CreateLink(type,null,null,null,null)
    .Request()
    .PostAsync();

```