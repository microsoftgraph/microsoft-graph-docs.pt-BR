---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4a2206ca1df6add49f2d30cacf053e46f28ffcd0
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/17/2021
ms.locfileid: "50274903"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var @string = await graphClient.Education.Classes["11012"].Assignments["19002"]
    .GetResourcesFolderUrl()
    .Request()
    .GetAsync();

```