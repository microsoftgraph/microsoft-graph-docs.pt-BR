---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1100eb3ce1461af0c6134ad94055d13f308aba13
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443299"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/profile/account/{id}')
    .version('beta')
    .get();

```