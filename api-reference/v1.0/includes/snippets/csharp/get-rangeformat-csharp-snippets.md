---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 82bb840784bb1674f3456541a91a4389b2b68b98
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35740154"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRangeFormat = await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"].Range().Format
    .Request()
    .GetAsync();

```