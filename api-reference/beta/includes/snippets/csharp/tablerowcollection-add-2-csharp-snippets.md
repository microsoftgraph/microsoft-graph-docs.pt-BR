---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7784fbdfabbe477ffaaf18b611446830baee84e19cbca8183324dec827fdfe23
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158251"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

Int32? index = null;

var values = JsonDocument.Parse("[[1,2,3],[4,5,6]]");

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Tables["{workbookTable-id}"].Rows
    .Add(index,values)
    .Request()
    .PostAsync();

```