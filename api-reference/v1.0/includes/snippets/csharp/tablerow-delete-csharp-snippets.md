---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8cbfd8a1094e2e9cf3d1fedc1a92a4fd9c1fc635
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50774806"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Tables["{workbookTable-id}"].Rows["{workbookTableRow-id}"]
    .Request()
    .DeleteAsync();

```