---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 672ec71879101810db62196e93b61fa83f4e1d77
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35507529"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var notebook = await graphClient.Me.Onenote.Notebooks["{id}"]
    .Request()
    .GetAsync();

```