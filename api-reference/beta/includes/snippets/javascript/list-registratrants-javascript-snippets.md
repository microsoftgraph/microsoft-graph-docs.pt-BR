---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 25538233be9fd642b034364bb52462eebfb2a032
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/23/2021
ms.locfileid: "60561052"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let registrants = await client.api('/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ/registration/registrants')
    .version('beta')
    .get();

```