---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 82bb840784bb1674f3456541a91a4389b2b68b98
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35498251"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRangeFormat = await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"].Range().Format
    .Request()
    .GetAsync();

```