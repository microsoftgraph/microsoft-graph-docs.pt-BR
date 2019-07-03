---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c56cc4e70ae3a7024732f06ac19b7fd845208a38
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35517930"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/publish')
    .version('beta')
    .post();

```