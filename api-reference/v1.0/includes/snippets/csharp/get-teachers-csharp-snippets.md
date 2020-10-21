---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cffef970a55583a79202d9b31a5d0d75c8b535dd
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48612843"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var teachers = await graphClient.Education.Classes["{class-id}"].Teachers
    .Request()
    .GetAsync();

```