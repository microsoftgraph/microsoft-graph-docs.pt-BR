---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 647e88f13e1e6a7ed5eb34ce25d4fd3581c70064
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62137578"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/bookingBusinesses/Contosolunchdelivery@contoso.onmicrosoft.com/publish')
    .version('beta')
    .post();

```