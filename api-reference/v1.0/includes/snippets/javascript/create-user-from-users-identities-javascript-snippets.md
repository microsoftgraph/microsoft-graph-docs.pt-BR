---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8934fb250a064f032be09e29b227047f9df57b7e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50785654"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const user = {
  displayName: 'John Smith',
  identities: [
    {
      signInType: 'userName',
      issuer: 'contoso.onmicrosoft.com',
      issuerAssignedId: 'johnsmith'
    },
    {
      signInType: 'emailAddress',
      issuer: 'contoso.onmicrosoft.com',
      issuerAssignedId: 'jsmith@yahoo.com'
    },
    {
      signInType: 'federated',
      issuer: 'facebook.com',
      issuerAssignedId: '5eecb0cd'
    }
  ],
  passwordProfile: {
    password: 'password-value',
    forceChangePasswordNextSignIn: false
  },
  passwordPolicies: 'DisablePasswordExpiration'
};

await client.api('/users')
    .post(user);

```