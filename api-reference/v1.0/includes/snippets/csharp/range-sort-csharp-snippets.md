---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 264b737a7965f3da23c5a96470fcdc3b1792dcb1e7520412a0cf38d67389eebc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100224"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRangeSort = await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Names["{workbookNamedItem-id}"]
    .Range().Sort
    .Request()
    .GetAsync();

```