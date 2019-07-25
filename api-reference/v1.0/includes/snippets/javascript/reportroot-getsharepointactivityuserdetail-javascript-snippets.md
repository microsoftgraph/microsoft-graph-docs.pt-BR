---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cb22b052fe43e8aefcd8f9a1b3105734420576a6
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35730907"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getSharePointActivityUserDetail(period='D7')')
    .get();

```