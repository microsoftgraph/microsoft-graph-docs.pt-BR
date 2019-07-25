---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 23db8bf9f3dbe6662f430e02d8106c5199bca6a3
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35710956"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessReview = await graphClient.AccessReviews["2b83cc42-09db-46f6-8c6e-16fec466a82d"]
    .Request()
    .GetAsync();

```