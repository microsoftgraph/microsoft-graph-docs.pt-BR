---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a6cebbf163ebd3782d751a6ac9642bce6c2faf37bd48f65dfc9891f346d3ac7b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57327021"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const transfer = {
  transferTarget: {
    '@odata.type': '#microsoft.graph.invitationParticipantInfo',
    endpointType: 'default',
    identity: {
      '@odata.type': '#microsoft.graph.identitySet',
      user: {
        '@odata.type': '#microsoft.graph.identity',
        id: '550fae72-d251-43ec-868c-373732c2704f',
        tenantId: '72f988bf-86f1-41af-91ab-2d7cd011db47',
        displayName: 'Heidi Steen'
      }
    },
    languageId: 'en-us',
    region: 'amer',
    replacesCallId: 'e5d39592-99bd-4db8-bca8-30fb894ec51d'
  }
};

await client.api('/communications/calls/341a0500-d4bf-4224-8b19-1581168d328b/transfer')
    .version('beta')
    .post(transfer);

```