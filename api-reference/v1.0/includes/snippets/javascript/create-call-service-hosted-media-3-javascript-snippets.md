---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4ec64fe528f6a4a531dc6a9548b79885fbd982a2efc5741deb7c5ac57e7184a9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57217124"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const call = {
  '@odata.type': '#microsoft.graph.call',
  callbackUri: 'https://bot.contoso.com/callback',
  source: {
    '@odata.type': '#microsoft.graph.participantInfo',
    identity: {
      '@odata.type': '#microsoft.graph.identitySet',
      applicationInstance: {
        '@odata.type': '#microsoft.graph.identity',
        displayName: 'Calling Bot',
        id: '3d913abb-aec0-4964-8fa6-3c6850c4f278'
      },
    },
    countryCode: null,
    endpointType: null,
    region: null,
    languageId: null
  },
  targets: [
    {
      '@odata.type': '#microsoft.graph.invitationParticipantInfo',
      identity: {
        '@odata.type': '#microsoft.graph.identitySet',
        phone: {
          '@odata.type': '#microsoft.graph.identity',
          id: '+12345678901'
        }
      }
    }
  ],
  requestedModalities: [
    'audio'
  ],
  mediaConfig: {
    '@odata.type': '#microsoft.graph.appHostedMediaConfig',
    blob: '<Media Session Configuration>'
  },
  tenantId: 'aa67bd4c-8475-432d-bd41-39f255720e0a'
};

await client.api('/communications/calls')
    .post(call);

```