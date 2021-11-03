---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 92dd684e57a3969eae3d8b41798402ef1fe16da0
ms.sourcegitcommit: 64d27a0e3dcccc9d857e62aace4153e5d98fb3d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60730372"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let recoveryKeys = await client.api('/informationProtection/bitlocker/recoveryKeys')
    .header('ocp-client-name','"My Friendly Client"')
    .header('ocp-client-version','"1.2"')
    .get();

```