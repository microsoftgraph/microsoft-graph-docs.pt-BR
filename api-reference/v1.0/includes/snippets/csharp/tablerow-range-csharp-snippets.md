---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 23c29ee7b51e88472223bda23947bc43bf6399a2
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35739840"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Items["{id}"].Workbook.Tables["{id|name}"].Rows["{index}"].Range()
    .Request()
    .GetAsync();

```