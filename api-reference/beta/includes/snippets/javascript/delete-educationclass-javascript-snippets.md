---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a53b1c1d0a4c51ecacb696cdc58e6ddd7f73c0c8
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50782621"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/education/classes/11022')
    .version('beta')
    .delete();

```