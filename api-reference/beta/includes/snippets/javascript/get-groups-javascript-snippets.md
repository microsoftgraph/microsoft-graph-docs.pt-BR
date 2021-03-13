---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cc51671dcc5e78d259c1c57b2829653839ed5f6b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50787680"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let groups = await client.api('/groups')
    .version('beta')
    .get();

```