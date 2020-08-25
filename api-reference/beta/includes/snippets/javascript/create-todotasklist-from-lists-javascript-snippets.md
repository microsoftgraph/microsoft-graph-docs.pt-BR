---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4807ae8323d472f46cdf337de523e9185b53f54a
ms.sourcegitcommit: ef47b165f7a140cfc0309a275cb8722dd265660d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/25/2020
ms.locfileid: "46872857"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const lists = {
  displayName: "Travel items",
};

let res = await client.api('/me/todo/lists')
    .version('beta')
    .post(lists);

```