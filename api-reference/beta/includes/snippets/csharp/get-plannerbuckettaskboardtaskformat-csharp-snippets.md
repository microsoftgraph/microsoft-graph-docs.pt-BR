---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: db4c13d8b3bd2fd94e34ce6dc45c486733b9167e
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48603840"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plannerBucketTaskBoardTaskFormat = await graphClient.Planner.Tasks["01gzSlKkIUSUl6DF_EilrmQAKDhh"].BucketTaskBoardFormat
    .Request()
    .GetAsync();

```