---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cfcdf0f03ada674e169315da651e80e5ca10a938
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48618789"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var names = await graphClient.Me.Drive.Items["{id}"].Workbook.Names
    .Request()
    .GetAsync();

```