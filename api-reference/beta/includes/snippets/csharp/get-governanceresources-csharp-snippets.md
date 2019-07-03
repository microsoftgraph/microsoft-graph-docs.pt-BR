---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 566c1d0aa99bcf0ffd5b766cf4af45b8459f1468
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35498430"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var resources = await graphClient.PrivilegedAccess["azureResources"].Resources
    .Request()
    .GetAsync();

```