---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 58edc3fc484edd3a09846f6c06599bf1fe8a598c5480af15229240b43be8e461
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159924"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const itemEmail = {
  address: 'Innocenty.Popov@adventureworks.com',
};

await client.api('/me/profile/emails')
    .version('beta')
    .post(itemEmail);

```