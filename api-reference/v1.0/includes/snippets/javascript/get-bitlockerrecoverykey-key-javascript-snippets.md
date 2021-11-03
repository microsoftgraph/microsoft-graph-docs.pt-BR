---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bf09bdec7949030b78db04c3bf2bcad911404adf
ms.sourcegitcommit: 64d27a0e3dcccc9d857e62aace4153e5d98fb3d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60729889"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let bitlockerRecoveryKey = await client.api('/informationProtection/bitlocker/recoveryKeys/b465e4e8-e4e8-b465-e8e4-65b4e8e465b4')
    .select('key')
    .get();

```