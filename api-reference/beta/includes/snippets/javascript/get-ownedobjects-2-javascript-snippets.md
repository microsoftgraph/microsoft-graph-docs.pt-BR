---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 672ddec2bbdc5a181ab18c0a21d9f4ea12b1e25b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960509"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let ownedObjects = await client.api('/me/ownedObjects')
    .version('beta')
    .get();

```