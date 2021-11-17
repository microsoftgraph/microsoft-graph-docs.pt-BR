---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: aa4e4911d19e6a8b5cb04b86a26b7ca355c6ee3083e399a2241b8a61ca24d695
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57327993"
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
    .version('beta')
    .post(user);

```