---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 090b8fe6f0c9beb538771addac3a3caae28170228ea5a6ae9eba5f72abeb8e4b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57099818"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const accessReviewHistoryDefinition = {
  displayName: 'Last quarter\'s group reviews April 2021',
  decisions: [
    'approve',
    'deny',
    'dontKnow',
    'notReviewed',
    'notNotified'
  ],
  reviewHistoryPeriodStartDateTime: '2021-01-01T00:00:00Z',
  reviewHistoryPeriodEndDateTime: '2021-04-05T00:00:00Z',
  scopes: [
    {
      '@odata.type': '#microsoft.graph.accessReviewQueryScope',
      queryType: 'MicrosoftGraph',     
      query: '/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, \'accessPackageAssignments\')',
      queryRoot: null
    },  
    {
      '@odata.type': '#microsoft.graph.accessReviewQueryScope',
      queryType: 'MicrosoftGraph',     
      query: '/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, \'/groups\')',
      queryRoot: null
    }
  ]
};

await client.api('/identityGovernance/accessReviews/historyDefinitions')
    .version('beta')
    .post(accessReviewHistoryDefinition);

```