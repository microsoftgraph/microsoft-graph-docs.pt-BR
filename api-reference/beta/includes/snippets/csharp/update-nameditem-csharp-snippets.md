---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0487e5890412a25def34cfa41507542f609bd32864d31bff92dc92efa3c03411
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102612"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookNamedItem = new WorkbookNamedItem
{
    Type = "type-value",
    Scope = "scope-value",
    Comment = "comment-value",
    Value = JsonDocument.Parse("{}"),
    Visible = true
};

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Names["{workbookNamedItem-id}"]
    .Request()
    .UpdateAsync(workbookNamedItem);

```