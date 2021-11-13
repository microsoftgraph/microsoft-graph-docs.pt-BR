---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fcfb218cee272e8f8f9028279e9fdcf7dec45157
ms.sourcegitcommit: c6a8c1cc13ace38d6c4371139ee84707c5c93352
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2021
ms.locfileid: "60890708"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var assignments = await graphClient.Education.Classes["{educationClass-id}"].Assignments
    .Request()
    .Expand("resources")
    .GetAsync();

```