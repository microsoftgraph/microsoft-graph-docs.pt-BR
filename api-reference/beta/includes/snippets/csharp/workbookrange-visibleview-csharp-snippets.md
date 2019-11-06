---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2a8566a1dcb037144d904df0e5d87df360258e8b
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37996140"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRangeView = await graphClient.Drive.Root.Workbook.Worksheets["{id}"]
    .Range("A1:Z10")
    .VisibleView()
    .Request()
    .GetAsync();

```