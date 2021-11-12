---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f57136675b9188a4d1e409ab1d5386118320c4451cd3b755f75a0f041e0e5733
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159920"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRangeBorder = new WorkbookRangeBorder
{
    Color = "color-value",
    Style = "style-value",
    SideIndex = "sideIndex-value",
    Weight = "weight-value"
};

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Names["{workbookNamedItem-id}"]
    .Range().Format.Borders["{workbookRangeBorder-id}"]
    .Request()
    .UpdateAsync(workbookRangeBorder);

```