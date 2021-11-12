---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 72b6a6b4bc654ba2383b9949dd62c3c836a49a08aa5c28be2a7a4099e6826097
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273351"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/education/users/delta')
    .version('beta')
    .get();

```