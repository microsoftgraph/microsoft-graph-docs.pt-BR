---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 41d6970297db80ad5777eb141ff29703e8acbde3
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50953101"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let history = await client.api('/riskyUsers/41a31b00-3b3b-42d9-8f1c-6d4f14e74c69/history')
    .version('beta')
    .get();

```