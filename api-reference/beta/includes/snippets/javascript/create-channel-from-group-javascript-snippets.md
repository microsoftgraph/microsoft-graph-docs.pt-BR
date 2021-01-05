---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 051b8cdac191cd3a6e31d3cd7465d21c1645930e
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/05/2021
ms.locfileid: "49753795"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const channel = {
  displayName: "Architecture Discussion",
  description: "This channel is where we debate all future architecture plans",
  membershipType: "standard"
};

let res = await client.api('/teams/57fb72d0-d811-46f4-8947-305e6072eaa5/channels')
    .version('beta')
    .post(channel);

```