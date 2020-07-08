---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: efeb30a66a0aa59d3a67588bae162b02d4d3eb28
ms.sourcegitcommit: 2050639c9e9a6b2dab9ce53d6a9fc87e98789b50
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/08/2020
ms.locfileid: "45081319"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const user = {
  displayName: "John Smith",
  identities: [
    {
      signInType: "userName",
      issuer: "contoso.onmicrosoft.com",
      issuerAssignedId: "johnsmith"
    },
    {
      signInType: "emailAddress",
      issuer: "contoso.onmicrosoft.com",
      issuerAssignedId: "jsmith@yahoo.com"
    },
    {
      signInType: "federated",
      issuer: "facebook.com",
      issuerAssignedId: "5eecb0cd"
    }
  ],
  "passwordProfile" : {
    password: "password-value",
    forceChangePasswordNextSignIn: false
  },
  passwordPolicies: "DisablePasswordExpiration"
};

let res = await client.api('/users')
    .post(user);

```