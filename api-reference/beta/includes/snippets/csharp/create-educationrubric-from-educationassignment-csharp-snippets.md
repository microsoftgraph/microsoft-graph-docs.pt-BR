---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 81b356f2f6d74896cc649b78f272416a17cac03f
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48966498"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.Classes["{id}"].Assignments["{id}"].Rubric.Reference
    .Request()
    .PutAsync("{id}");

```