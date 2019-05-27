---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bc28759d2c021ee8556f06b9bdd5770c5ca91b95
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34452753"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var applyTo = "applyTo-value";

await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"]
    .Range()
    .Clear(applyTo)
    .Request()
    .PostAsync();

```