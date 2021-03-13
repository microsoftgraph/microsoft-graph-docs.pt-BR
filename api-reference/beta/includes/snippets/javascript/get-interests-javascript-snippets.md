---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 35df34671f57359eba7111447379abf950d71b72
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50804102"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let interests = await client.api('/me/profile/interests')
    .version('beta')
    .get();

```