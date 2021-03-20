---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bca416a25f0c369b15c1e133b54e5f0a31ac84ae
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50942157"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const tiIndicator = {
  description: 'description-updated',
};

await client.api('/security/tiIndicators/{id}')
    .version('beta')
    .update(tiIndicator);

```