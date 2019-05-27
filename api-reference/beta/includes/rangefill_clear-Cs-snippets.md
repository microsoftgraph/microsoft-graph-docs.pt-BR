---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b769552d0b9b860d4a6aa802b799411d15318708
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34442673"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"]
    .Range().Format.Fill
    .Clear()
    .Request()
    .PostAsync();

```