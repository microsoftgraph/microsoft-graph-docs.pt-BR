---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d7fb16814145853aac047097cc07657391097a973cbf6dc0d5736deaf8c0dfb3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57271876"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Worksheets["{workbookWorksheet-id}"]
    .UsedRange()
    .Request()
    .GetAsync();

```