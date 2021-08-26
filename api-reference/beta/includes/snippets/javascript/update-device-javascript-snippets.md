---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0448fa91b62e439c822b87c4af505fd8530fa2e992f643dd95d81d04b4d65eaf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57326885"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const device = {
  accountEnabled: false
};

await client.api('/devices/{id}')
    .version('beta')
    .update(device);

```