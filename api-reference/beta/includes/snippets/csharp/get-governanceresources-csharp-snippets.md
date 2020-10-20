---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 566c1d0aa99bcf0ffd5b766cf4af45b8459f1468
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48619613"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var resources = await graphClient.PrivilegedAccess["azureResources"].Resources
    .Request()
    .GetAsync();

```