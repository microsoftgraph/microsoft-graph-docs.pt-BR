---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: aa9cf9979caec3610f5b3f66beb5f9f7a9146a3ca7703ed1b8f44f438b715347
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102694"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const forward = {
  comment: 'comment-value',
  toRecipients: [
    {
      emailAddress: {
        name: 'name-value',
        address: 'address-value'
      }
    }
  ]
};

await client.api('/me/messages/{id}/forward')
    .post(forward);

```