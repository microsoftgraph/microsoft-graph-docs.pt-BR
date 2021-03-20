---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fe6d5100e659b882986256133aedafdad8158793
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50950491"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const confirmCompromised = {
  userIds: [
    '29f270bb-4d23-4f68-8a57-dc73dc0d4caf'
  ]
};

await client.api('/identityProtection/riskyUsers/confirmCompromised')
    .version('beta')
    .post(confirmCompromised);

```