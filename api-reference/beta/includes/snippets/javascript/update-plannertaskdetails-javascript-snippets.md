---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4dbcc705b9a712cf7caeb9da094f27446a6a7af2e6286273c9eed6236c7bb3f7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57217165"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const plannerTaskDetails = {
  previewType: 'noPreview',
  references: {
    'http%3A//developer%2Emicrosoft%2Ecom':{
      '@odata.type': 'microsoft.graph.plannerExternalReference',
      alias: 'Documentation',
      previewPriority: ' !',
      type: 'Other'
    },
    'https%3A//developer%2Emicrosoft%2Ecom/en-us/graph/graph-explorer':{
      '@odata.type': 'microsoft.graph.plannerExternalReference',
      previewPriority: '  !!',
    },
    'http%3A//www%2Ebing%2Ecom': null
  },
  checklist: {
    '95e27074-6c4a-447a-aa24-9d718a0b86fa':{
      '@odata.type': 'microsoft.graph.plannerChecklistItem',
      title: 'Update task details',
      isChecked: true
    },
    'd280ed1a-9f6b-4f9c-a962-fb4d00dc50ff':{
      '@odata.type': 'microsoft.graph.plannerChecklistItem',
      isChecked: true,
    },
    'a93c93c5-10a6-4167-9551-8bafa09967a7': null
  }
};

await client.api('/planner/tasks/gcrYAaAkgU2EQUvpkNNXLGQAGTtu/details')
    .version('beta')
    .update(plannerTaskDetails);

```