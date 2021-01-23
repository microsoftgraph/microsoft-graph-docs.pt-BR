---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f428ae4b14b09e2f369eba8c5aa1d63c940f7c50
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2021
ms.locfileid: "49945364"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/identityProviders/{id}')
    .version('beta')
    .get();

```