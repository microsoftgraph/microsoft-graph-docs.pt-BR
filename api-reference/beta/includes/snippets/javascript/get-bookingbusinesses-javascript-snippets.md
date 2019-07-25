---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a9b8cae5c796eddb52b507e63199176a2d3845ef
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35709863"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/bookingBusinesses')
    .version('beta')
    .get();

```