---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 41bb3fca0f5eba101ccf99801d075b88981b524a
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59765674"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let device = await client.api('/devices/000005c3-b7a6-4c61-89fc-80bf5ccfc366')
    .version('beta')
    .get();

```