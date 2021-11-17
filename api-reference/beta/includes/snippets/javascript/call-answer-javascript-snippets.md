---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: af6b3bf4c2cd93177084cbb0e20ba162fb2b9d1dbbaf781536697e4a95096196
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159713"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const answer = {
  callbackUri: 'callbackUri-value',
  mediaConfig: {
    '@odata.type': '#microsoft.graph.appHostedMediaConfig',
    blob: '<Media Session Configuration Blob>'
  },
  acceptedModalities: [
    'audio'
  ],
  participantCapacity: 200
};

await client.api('/communications/calls/{id}/answer')
    .version('beta')
    .post(answer);

```