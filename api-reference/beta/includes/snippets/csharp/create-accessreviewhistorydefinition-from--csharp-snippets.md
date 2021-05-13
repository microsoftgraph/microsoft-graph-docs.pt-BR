---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 422a97a5851ee8a5e3be2f099764112034f8ef97
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2021
ms.locfileid: "52474110"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessReviewHistoryDefinition = new AccessReviewHistoryDefinition
{
    DisplayName = "Last quarter's group reviews April 2021",
    Decisions = new List<AccessReviewHistoryDecisionFilter>()
    {
        AccessReviewHistoryDecisionFilter.Approve,
        AccessReviewHistoryDecisionFilter.Deny,
        AccessReviewHistoryDecisionFilter.DontKnow,
        AccessReviewHistoryDecisionFilter.NotReviewed,
        AccessReviewHistoryDecisionFilter.NotNotified
    },
    ReviewHistoryPeriodStartDateTime = DateTimeOffset.Parse("2021-01-01T00:00:00Z"),
    ReviewHistoryPeriodEndDateTime = DateTimeOffset.Parse("2021-04-05T00:00:00Z"),
    Scopes = new List<AccessReviewScope>()
    {
        new AccessReviewQueryScope
        {
            QueryType = "MicrosoftGraph",
            Query = "/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, 'accessPackageAssignments')",
            QueryRoot = null
        },
        new AccessReviewQueryScope
        {
            QueryType = "MicrosoftGraph",
            Query = "/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, '/groups')",
            QueryRoot = null
        }
    }
};

await graphClient.IdentityGovernance.AccessReviews.HistoryDefinitions
    .Request()
    .AddAsync(accessReviewHistoryDefinition);

```