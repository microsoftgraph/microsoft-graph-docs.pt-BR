---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 891221f1af67055896368cea41201387521b8e3b
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2020
ms.locfileid: "46569984"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const confirmCompromised = {
  userIds: [
    "29f270bb-4d23-4f68-8a57-dc73dc0d4caf"
  ]
};

let res = await client.api('/identityProtection/riskyUsers/confirmCompromised')
    .version('beta')
    .post(confirmCompromised);

```