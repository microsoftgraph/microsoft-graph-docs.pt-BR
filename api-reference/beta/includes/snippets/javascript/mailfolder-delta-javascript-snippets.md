---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 21c02989a6b0b73fb664a924a2c845b11741b7bd
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800549"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/me/mailFolders/delta')
    .version('beta')
    .get();

```