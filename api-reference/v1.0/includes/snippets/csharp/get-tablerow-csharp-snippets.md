---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6339b4df6f02e55b8ae6d9f13533df1bc58cf64cf59405cb9bc0ed5c86a27fc8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329676"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookTableRow = await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Tables["{workbookTable-id}"].Rows["{workbookTableRow-id}"]
    .Request()
    .GetAsync();

```