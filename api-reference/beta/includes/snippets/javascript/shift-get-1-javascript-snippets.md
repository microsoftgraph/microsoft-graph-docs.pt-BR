---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 34dc979b41d075b1951693aea9eb38a760a404b1e6ead5136d9d1ff67e908ffd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329255"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let shift = await client.api('/teams/{teamId}/schedule/shifts/{shiftId}')
    .version('beta')
    .get();

```