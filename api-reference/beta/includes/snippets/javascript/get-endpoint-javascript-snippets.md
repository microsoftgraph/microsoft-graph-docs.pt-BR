---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 43a14c1d49017d30062a3ab4dc8b457bc7046b34a2a5ad83b3a2bd9ac9ff2613
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157927"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let endpoint = await client.api('/groups/{id}/endpoints/{id}')
    .version('beta')
    .get();

```