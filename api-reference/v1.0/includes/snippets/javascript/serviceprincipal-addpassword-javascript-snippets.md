---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a96bc7eb26d5e6c826d8c4e7a42a44bdb128c8aa
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/21/2020
ms.locfileid: "44334407"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const passwordCredential = {
  passwordCredential: {
    displayName: "Password friendly name"
  }
};

let res = await client.api('/servicePrincipals/{id}/addPassword')
    .post(passwordCredential);

```