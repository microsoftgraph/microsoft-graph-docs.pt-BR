---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 52edce7be4867baa2710b6d69a7cf3fa44b21a9a
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35466362"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var domains = await graphClient.Domains
    .Request()
    .GetAsync();

```