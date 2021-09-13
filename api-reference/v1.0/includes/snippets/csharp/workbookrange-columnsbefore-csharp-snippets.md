---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c3e2aa68aa51a56256ae29ac6dd4679d9938c7e5a8ee5f359c99f57448cd7c2e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216067"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Root.Workbook.Worksheets["{workbookWorksheet-id}"]
    .Range()
    .ColumnsBefore(2)
    .Request()
    .GetAsync();

```