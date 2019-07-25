---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fd4e37eaf180fbab4aa5e718c6ae4705b577d3a4
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35859174"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookFormatProtection = new WorkbookFormatProtection
{
    Locked = true,
    FormulaHidden = true
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"]
    .Range().Format.Protection
    .Request()
    .UpdateAsync(workbookFormatProtection);

```