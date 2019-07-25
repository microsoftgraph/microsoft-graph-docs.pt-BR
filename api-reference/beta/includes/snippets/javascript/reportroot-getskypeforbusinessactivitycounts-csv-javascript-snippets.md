---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 96ea3489b37264c11ad76837bb7ecf8dcc8dff66
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35726915"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getSkypeForBusinessActivityCounts(period='D7')')
    .version('beta')
    .get();

```