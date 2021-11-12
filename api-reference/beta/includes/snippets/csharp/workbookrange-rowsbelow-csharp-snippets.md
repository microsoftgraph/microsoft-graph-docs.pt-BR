---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 48428fed29aea0f9b0174737be2fc8684dc723f13446ad2d75cb46ff996b2153
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216818"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Drive.Root.Workbook.Worksheets["{workbookWorksheet-id}"]
    .Range()
    .RowsBelow(2)
    .Request()
    .GetAsync();

```