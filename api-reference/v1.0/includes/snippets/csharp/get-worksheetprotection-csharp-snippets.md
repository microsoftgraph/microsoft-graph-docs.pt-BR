---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 21bb1b8c6ce7b8aab53b513e70944b8ccc4f4176d55bc26ad46943c856b14ea4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57271873"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookWorksheetProtection = await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Worksheets["{workbookWorksheet-id}"].Protection
    .Request()
    .GetAsync();

```