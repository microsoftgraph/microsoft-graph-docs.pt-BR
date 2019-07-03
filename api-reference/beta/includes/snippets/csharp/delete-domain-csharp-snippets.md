---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: eb143d00ead236726b37b1e8f2d29d4106a1d476
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35517590"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Domains["contoso.com"]
    .Request()
    .DeleteAsync();

```