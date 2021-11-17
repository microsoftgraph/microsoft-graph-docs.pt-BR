---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 29963b1e0fe6c4dfdb2826f7ae1c5113a22abd1c49c47ddd15580f74ee85b471
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273184"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let tokenLifetimePolicies = await client.api('/policies/tokenLifetimePolicies')
    .version('beta')
    .get();

```