---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7be7ce1e54ca689d2df5e72e7dd71a9036db7ac3549c528bafde84aba5cafe53
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57099430"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const user = {
  accountEnabled: true,
  displayName: 'Adele Vance',
  mailNickname: 'AdeleV',
  userPrincipalName: 'AdeleV@contoso.onmicrosoft.com',
  passwordProfile: {
    forceChangePasswordNextSignIn: true,
    password: 'xWwvJ]6NMw+bWH-d'
  }
};

await client.api('/users')
    .post(user);

```