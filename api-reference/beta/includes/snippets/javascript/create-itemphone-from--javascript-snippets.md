---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 08b3fecaeaeeee0f890797a2f1bf8e96a710ddb0
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50801095"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const itemPhone = {
  displayName: 'Car Phone',
  number: '+7 499 342 22 13'
};

await client.api('/me/profile/phones')
    .version('beta')
    .post(itemPhone);

```