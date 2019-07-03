---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 23c29ee7b51e88472223bda23947bc43bf6399a2
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35507710"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Items["{id}"].Workbook.Tables["{id|name}"].Rows["{index}"].Range()
    .Request()
    .GetAsync();

```