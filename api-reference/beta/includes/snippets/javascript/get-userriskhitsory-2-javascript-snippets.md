---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7c46a79f31d2cb89d6a3e9481867303f29a7c23a
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50953107"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let history = await client.api('/identityProtection/riskyUsers/41a31b00-3b3b-42d9-8f1c-6d4f14e74c69/history')
    .version('beta')
    .get();

```