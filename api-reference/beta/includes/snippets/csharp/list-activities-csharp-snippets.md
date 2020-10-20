---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 360ebe3b06dcd09e484bff21fe3637cf7772d6ad
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48612437"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var activities = await graphClient.Me.Drive.Activities
    .Request()
    .GetAsync();

```