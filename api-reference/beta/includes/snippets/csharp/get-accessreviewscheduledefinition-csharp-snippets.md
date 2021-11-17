---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e49333d1489b6fe62f79f0fb13ef13656716984ddf6164a2b3ea8e047eecf2f8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56898144"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessReviewScheduleDefinition = await graphClient.IdentityGovernance.AccessReviews.Definitions["{accessReviewScheduleDefinition-id}"]
    .Request()
    .GetAsync();

```