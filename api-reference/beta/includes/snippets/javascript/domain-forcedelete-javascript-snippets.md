---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8df580e4ccae33a089091189eb0b8615c28eecdf
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800090"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const forceDelete = {
  disableUserAccounts: true
};

await client.api('/domains/contoso.com/forceDelete')
    .version('beta')
    .post(forceDelete);

```