---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 75f7520168efc41d7329d9b4a8955a134c6aefd98daadf2e1acefc6715d219ba
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273291"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let notebooks = await client.api('/me/onenote/notebooks')
    .version('beta')
    .get();

```