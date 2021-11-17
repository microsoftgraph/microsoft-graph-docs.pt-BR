---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ccf0b713a90ed2152d2ad0042038ce3078bcb7cc1267f16defec474f80fc5ec1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57213639"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const passwordCredential = {
  passwordCredential: {
    displayName: 'Password friendly name'
  }
};

await client.api('/applications/{id}/addPassword')
    .version('beta')
    .post(passwordCredential);

```