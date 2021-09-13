---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ced4a6535c92c1ecabb8f50f62a5b9c20466236ef8dc126cae18f737fe04ed9b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158062"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var index = 5;

var values = JsonDocument.Parse("[[1,2,3],[4,5,6]]");

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Tables["{workbookTable-id}"].Rows
    .Add(index,values)
    .Request()
    .PostAsync();

```