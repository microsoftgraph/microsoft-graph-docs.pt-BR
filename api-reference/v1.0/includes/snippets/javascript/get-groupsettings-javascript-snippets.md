---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: aa2cfd48409722c7f55e5c84908f9f337311eb87
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50805527"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let groupSettings = await client.api('/groupSettings')
    .get();

```