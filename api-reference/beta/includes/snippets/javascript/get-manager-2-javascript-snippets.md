---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b01c1152ac9f4c19d039fce11d377cfb27d1e621
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50957098"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let directoryObject = await client.api('/users/{id|userPrincipalName}/manager')
    .version('beta')
    .get();

```