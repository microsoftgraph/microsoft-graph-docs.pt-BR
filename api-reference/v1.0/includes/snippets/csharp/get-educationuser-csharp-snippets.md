---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ebe7989c3ff5d85546aca4413499854b072c26ac
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35492460"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationUser = await graphClient.Education.Users["{user-id}"]
    .Request()
    .GetAsync();

```