---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: acf7241d7d565b234e15c34a3798e76193752cd4
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50787209"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/education/classes/11021/assignments/19002/resources/22002')
    .version('beta')
    .delete();

```