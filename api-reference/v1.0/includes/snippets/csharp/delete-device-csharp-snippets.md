---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ab8bde42fb4ca337230599efbf7c4da029724608
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35466199"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Devices["{id}"]
    .Request()
    .DeleteAsync();

```