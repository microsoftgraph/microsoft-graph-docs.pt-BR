---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 82bb840784bb1674f3456541a91a4389b2b68b98
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34446967"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRangeFormat = await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"].Range().Format
    .Request()
    .GetAsync();

```