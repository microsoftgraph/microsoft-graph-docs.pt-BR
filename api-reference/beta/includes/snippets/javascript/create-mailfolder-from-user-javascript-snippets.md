---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0a2558e74af4abacfdb5ebd70d45736fc8a185dd
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50809033"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const mailFolder = {
  displayName: 'Clutter',
  isHidden: true
};

await client.api('/me/mailFolders')
    .version('beta')
    .post(mailFolder);

```