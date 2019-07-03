---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 26b72e4a7ce9b9843def0f31363570d5579acf7b
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35499360"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Me.Planner.All.Delta()
    .Request()
    .GetAsync();

```