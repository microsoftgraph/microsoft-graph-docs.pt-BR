---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0543c1e018eedb394e9dd8a20365f3bac10ad44462d6a11306fad8bead0dd3cb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57156465"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const oAuth2PermissionGrant = {
  clientId: 'clientId-value',
  consentType: 'consentType-value',
  principalId: 'principalId-value',
  resourceId: 'resourceId-value',
  scope: 'scope-value',
  startTime: '2016-10-19T10:37:00Z',
  expiryTime: '2016-10-19T10:37:00Z'
};

await client.api('/oauth2PermissionGrants')
    .version('beta')
    .post(oAuth2PermissionGrant);

```