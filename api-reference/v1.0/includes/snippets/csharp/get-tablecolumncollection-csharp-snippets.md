---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cc23ce61c9a64e1474d25d8c0a4036eba7f48671
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35737473"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var columns = await graphClient.Me.Drive.Items["{id}"].Workbook.Tables["{id|name}"].Columns
    .Request()
    .GetAsync();

```