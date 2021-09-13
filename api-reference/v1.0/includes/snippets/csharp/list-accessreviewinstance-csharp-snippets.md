---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 71ec03f45eee86b676aadc050bbd145316d4f3e429c7aa7fdfe541186f1245e4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100691"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var instances = await graphClient.IdentityGovernance.AccessReviews.Definitions["{accessReviewScheduleDefinition-id}"].Instances
    .Request()
    .GetAsync();

```