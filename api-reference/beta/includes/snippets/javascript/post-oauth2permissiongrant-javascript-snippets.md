---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1fd8097841557a6588574041fce33297c81c9544
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50801663"
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