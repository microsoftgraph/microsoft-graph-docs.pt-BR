---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2bd3c4a1508312d9fdf2a816b3df5672825c12ad3e53988e9f1d1b39e1964d9d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899138"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let bookingBusinesses = await client.api('/bookingBusinesses?query=Adventure')
    .version('beta')
    .get();

```