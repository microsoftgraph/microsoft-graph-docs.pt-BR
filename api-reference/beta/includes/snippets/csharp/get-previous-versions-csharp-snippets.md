---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5899a66e621e2053b71f970de184b67ea5917c95
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48619206"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var versions = await graphClient.Me.Drive.Items["{item-id}"].Versions
    .Request()
    .GetAsync();

```