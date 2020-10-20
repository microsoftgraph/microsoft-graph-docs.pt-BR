---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b42a77581db41701eb4bbc7ecf0cfb1cb644c72b
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48618380"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var points = await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"].Charts["{name}"].Series["{undefined}"].Points
    .Request()
    .GetAsync();

```