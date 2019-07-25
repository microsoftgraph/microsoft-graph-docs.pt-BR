---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 36bb2d3d2a8b2317fc41f1fae6a1c4b53b6289c2
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35711747"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/subscribeByMail')
    .version('beta')
    .post();

```