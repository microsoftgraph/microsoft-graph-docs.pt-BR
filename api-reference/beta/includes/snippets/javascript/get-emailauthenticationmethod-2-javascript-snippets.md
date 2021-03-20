---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d5f518b8b07d78d19c55e7bc3e7177e0a537bcbe
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50950962"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let emailMethods = await client.api('/me/authentication/emailMethods')
    .version('beta')
    .get();

```