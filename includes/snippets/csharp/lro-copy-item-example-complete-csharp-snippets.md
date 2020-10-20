---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dc93bcaf0755ac9776f4e88ea0c754c09245f975
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48619127"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var driveItem = await graphClient.Me.Drive.Items["{item-id}"]
    .Request()
    .GetAsync();

```