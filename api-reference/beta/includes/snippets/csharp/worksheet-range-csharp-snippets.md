---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e890986b25b66c65121240c6b6c7b5a4e1f408d66755c89b92c5523075abe2cf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273500"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Worksheets["{workbookWorksheet-id}"]
    .Range()
    .Request()
    .GetAsync();

```