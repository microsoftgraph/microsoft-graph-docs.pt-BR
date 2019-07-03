---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 525f9daa8f70085ceec6c19ee0edce8a0b276e12
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35518129"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/customers')
    .version('beta')
    .get();

```