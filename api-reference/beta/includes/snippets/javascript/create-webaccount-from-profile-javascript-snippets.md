---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 38872d4c2e1bfbbdf52630b72a4e77cbaf519bb389c787a806a1f5139f1a0412
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159634"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const webAccount = {
  description: 'My Github contributions!',
  userId: 'innocenty.popov',
  service: {
    name: 'GitHub',
    webUrl: 'https://github.com'
  }
};

await client.api('/me/profile/webAccounts')
    .version('beta')
    .post(webAccount);

```