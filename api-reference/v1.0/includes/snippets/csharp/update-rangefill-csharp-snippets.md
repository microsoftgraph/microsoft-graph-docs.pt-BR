---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 98bbce25bfb155415b90efabb127b5093304c77ed99b2badabe67beb6e0f2a7b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157912"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRangeFill = new WorkbookRangeFill
{
    Color = "color-value"
};

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Names["{workbookNamedItem-id}"]
    .Range().Format.Fill
    .Request()
    .UpdateAsync(workbookRangeFill);

```