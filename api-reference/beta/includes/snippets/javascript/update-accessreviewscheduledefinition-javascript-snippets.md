---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1660774f159265026377f426c82fe830bff24e34
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60688063"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const accessReviewScheduleDefinition = {
  id: '60860cdd-fb4d-4054-91ba-f75e04444aa6',
  displayName: 'Test world UPDATED NAME!',
  descriptionForAdmins: 'Test world',
  descriptionForReviewers: 'Test world',
  scope: {
    '@odata.type': '#microsoft.graph.accessReviewQueryScope',
    query: '/groups/b7a059cb-038a-4802-8fc9-b9d1ed0cf11f/transitiveMembers',
    queryType: 'MicrosoftGraph'
  },
  instanceEnumerationScope: {
    '@odata.type': '#microsoft.graph.accessReviewQueryScope',
    query: '/groups/b7a059cb-038a-4802-8fc9-b9d1ed0cf11f',
    queryType: 'MicrosoftGraph'
  },
  reviewers: [],
  settings: {
    mailNotificationsEnabled: true,
    reminderNotificationsEnabled: true,
    justificationRequiredOnApproval: true,
    defaultDecisionEnabled: false,
    defaultDecision: 'None',
    instanceDurationInDays: 3,
    autoApplyDecisionsEnabled: false,
    recommendationsEnabled: true,
    recurrence: {
      pattern: {
        type: 'weekly',
        interval: 1
      },
      range: {
        type: 'noEnd',
        startDate: '2020-09-15'
      }
    }
  }
};

await client.api('/identityGovernance/accessReviews/definitions/60860cdd-fb4d-4054-91ba-f75e04444aa6')
    .version('beta')
    .put(accessReviewScheduleDefinition);

```