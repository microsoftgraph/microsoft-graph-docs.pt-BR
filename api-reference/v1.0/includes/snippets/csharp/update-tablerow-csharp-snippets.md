---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 05bd9db8f1c825722347b2ed619013affd1abf48fb7f94d318e1a82effa4b25f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57407011"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookTableRow = new WorkbookTableRow
{
    Index = 99,
    Values = JsonDocument.Parse(@"""values-value""")
};

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Tables["{workbookTable-id}"].Rows["{workbookTableRow-id}"]
    .Request()
    .UpdateAsync(workbookTableRow);

```