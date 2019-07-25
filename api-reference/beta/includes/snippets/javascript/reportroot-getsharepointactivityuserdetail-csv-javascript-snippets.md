---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dfe382db6b004822db3a808734edb059414cc379
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35727041"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getSharePointActivityUserDetail(period='D7')')
    .version('beta')
    .get();

```