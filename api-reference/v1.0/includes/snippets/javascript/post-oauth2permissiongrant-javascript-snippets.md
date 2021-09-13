---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b80873022d242eb00f4154115cb40bed2485f7fa6fdfc42387cfeb8f25a66e8b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57327116"
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
  scope: 'scope-value'
};

await client.api('/oauth2PermissionGrants')
    .post(oAuth2PermissionGrant);

```