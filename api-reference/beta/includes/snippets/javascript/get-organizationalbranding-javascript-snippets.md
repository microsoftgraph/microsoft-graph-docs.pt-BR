---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 19c95b05d5f0ba1f02423bead4cf95a9c396084b
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/23/2021
ms.locfileid: "60562739"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let organizationalBranding = await client.api('/organization/84841066-274d-4ec0-a5c1-276be684bdd3/branding')
    .version('beta')
    .header('Accept-Language','0')
    .get();

```