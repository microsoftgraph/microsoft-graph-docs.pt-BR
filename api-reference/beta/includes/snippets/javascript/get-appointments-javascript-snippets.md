---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3b0a48afcf5d942a5339d5fbaddc9d6409ceea55
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62109740"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let appointments = await client.api('/bookingBusinesses/Contosolunchdelivery@contoso.onmicrosoft.com/appointments')
    .version('beta')
    .get();

```