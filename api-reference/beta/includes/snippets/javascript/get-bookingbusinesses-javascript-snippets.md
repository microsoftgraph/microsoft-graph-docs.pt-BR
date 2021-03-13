---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 99355768eabea435b40d06cf92e0c8630633239b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50789411"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let bookingBusinesses = await client.api('/bookingBusinesses')
    .version('beta')
    .get();

```