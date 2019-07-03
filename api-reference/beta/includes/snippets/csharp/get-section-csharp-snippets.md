---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 32fc4220f0518c3708a92ae233f1879cb58c2468
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35498474"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var onenoteSection = await graphClient.Me.Onenote.Sections["{id}"]
    .Request()
    .GetAsync();

```