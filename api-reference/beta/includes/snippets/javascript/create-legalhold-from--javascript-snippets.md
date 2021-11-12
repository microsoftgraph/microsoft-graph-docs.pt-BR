---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6bdd44be21970c56ea49daed29c66da388dbdd22368fd1b2ee0336d4e3514526
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273364"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const legalHold = {
  '@odata.type': '#microsoft.graph.ediscovery.legalHold',
  description: 'String',
  createdBy: {
    '@odata.type': 'microsoft.graph.identitySet'
  },
  isEnabled: 'Boolean',
  status: 'String',
  contentQuery: 'String',
  errors: [
    'String'
  ],
  displayName: 'String'
};

await client.api('/compliance/ediscovery/cases/{caseId}/legalHolds')
    .version('beta')
    .post(legalHold);

```