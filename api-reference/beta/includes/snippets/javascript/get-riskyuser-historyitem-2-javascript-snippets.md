---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 331fb73885bd9796b907b2a5d661e02fe8871a70701090a671ac73fd2ccdae7e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899068"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let riskyUserHistoryItem = await client.api('/identityProtection/riskyUsers/41a31b00-3b3b-42d9-8f1c-6d4f14e74c69/history/41a31b00-3b3b-42d9-8f1c-6d4f14e74c69')
    .version('beta')
    .get();

```