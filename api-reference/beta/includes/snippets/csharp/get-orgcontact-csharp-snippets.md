---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 05db449e89d98c30d065c682c2fc041fb00c5886
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35477215"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var orgContact = await graphClient.Contacts["{id}"]
    .Request()
    .GetAsync();

```