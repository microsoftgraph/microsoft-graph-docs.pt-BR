---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3cbcacdd67447f03372527d4cda4ce80311709bd5b3e6ac434be9f509fe92397
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100863"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/settings/{id}')
    .version('beta')
    .delete();

```