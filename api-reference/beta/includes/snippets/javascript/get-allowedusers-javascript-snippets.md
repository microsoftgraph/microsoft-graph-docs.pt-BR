---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f3a92e8cb4f8cf4515730c273a6cec363e698c64
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50809580"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let allowedUsers = await client.api('/print/shares/{id}/allowedUsers')
    .version('beta')
    .get();

```