---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e81517e752eee35398ac1d5e08cc7aeec0702c2c
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50475802"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/authentication/temporaryAccessPassMethods')
    .version('beta')
    .get();

```