---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 54a5a70ea71a3cb83870a2c4f610b019ec109bf3
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35717229"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookTable = await graphClient.Me.Drive.Items["{id}"].Workbook.Tables["{id|name}"]
    .Request()
    .GetAsync();

```