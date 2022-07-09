---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c1ae2378e2166b3ff1155a3fc3c95c576f23bbf3
ms.sourcegitcommit: 6968f5aaf40089684efb0c38a95f6cca353c1d92
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/16/2022
ms.locfileid: "62853768"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var stages = await graphClient.IdentityGovernance.AccessReviews.Definitions["{accessReviewScheduleDefinition-id}"].Instances["{accessReviewInstance-id}"].Stages
    .Request()
    .GetAsync();

```