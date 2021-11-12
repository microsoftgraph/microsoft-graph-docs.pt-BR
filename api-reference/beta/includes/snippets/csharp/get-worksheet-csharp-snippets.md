---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 426c42a312e96f9f82bbf9ecd75ecb89dcda323fda57b84699128bca7ec04575
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899897"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookWorksheet = await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Worksheets["{workbookWorksheet-id}"]
    .Request()
    .GetAsync();

```