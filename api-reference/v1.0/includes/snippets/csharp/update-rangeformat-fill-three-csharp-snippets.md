---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 180a095ef021a2eabcab3111575c11abc9b837b8393c2c535810f13ceca0d541
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100999"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRangeFill = new WorkbookRangeFill
{
    Color = "#0000FF"
};

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Worksheets["{workbookWorksheet-id}"]
    .Range("$C$1").Format.Fill
    .Request()
    .UpdateAsync(workbookRangeFill);

```