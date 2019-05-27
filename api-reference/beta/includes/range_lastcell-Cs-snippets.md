---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 53c311b63425386faeec202eaa5324ade8e7f967
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34442841"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"].Range().LastCell()
    .Request()
    .GetAsync();

```