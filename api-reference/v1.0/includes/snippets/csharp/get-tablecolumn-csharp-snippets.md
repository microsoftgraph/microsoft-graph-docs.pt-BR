---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 66b170653f84b531d9f5735bf0350e75fb61f599241280ebb422f13823dca6f2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100981"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookTableColumn = await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Tables["{workbookTable-id}"].Columns["{workbookTableColumn-id}"]
    .Request()
    .GetAsync();

```