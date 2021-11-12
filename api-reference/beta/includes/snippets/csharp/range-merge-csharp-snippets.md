---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d8b6b843c2446de97e6350eeab56577691ba15074a13deaaf4f5c2f4ef6ccf03
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214523"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var across = true;

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Names["{workbookNamedItem-id}"]
    .Range()
    .Merge(across)
    .Request()
    .PostAsync();

```