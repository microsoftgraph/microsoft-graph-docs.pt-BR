---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ea68adbee33a6afc5a6a88c84cb890167776f6ee993ce2725abb215973957f08
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159524"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var filterByCurrentUser = await graphClient.IdentityGovernance.AccessReviews.Definitions
    .FilterByCurrentUser(AccessReviewScheduleDefinitionFilterByCurrentUserOptions.Reviewer)
    .Request()
    .GetAsync();

```