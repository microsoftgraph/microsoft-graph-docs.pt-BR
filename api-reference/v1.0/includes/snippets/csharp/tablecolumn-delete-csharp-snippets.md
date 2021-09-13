---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bd09dc3befebd0316d8860ad43856644518c5f23c111195937f839594d546834
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214712"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Tables["{workbookTable-id}"].Columns["{workbookTableColumn-id}"]
    .Request()
    .DeleteAsync();

```