---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fdad7eab666fd60fac0fb4ca3bc067a360b5a6f7
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50788813"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/groups/delta')
    .version('beta')
    .get();

```