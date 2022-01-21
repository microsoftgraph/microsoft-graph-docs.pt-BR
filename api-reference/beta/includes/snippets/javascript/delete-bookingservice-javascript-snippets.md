---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 699943c40c02dea424701c486540305867638387
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62116426"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/bookingBusinesses/Contosolunchdelivery@contoso.onmicrosoft.com/services/57da6774-a087-4d69-b0e6-6fb82c339976')
    .version('beta')
    .delete();

```