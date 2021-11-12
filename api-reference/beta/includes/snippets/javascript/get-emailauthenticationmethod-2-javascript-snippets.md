---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f9c1fc4b690d7832e241be243b1aeba84c5ea264ff21f8f3273c1b16563a11b1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102879"
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