---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a0e184b13541222cc4298a70bf452079f5d750dfdacc860100afc1cf1ef3342a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57213627"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/applications/delta')
    .version('beta')
    .get();

```