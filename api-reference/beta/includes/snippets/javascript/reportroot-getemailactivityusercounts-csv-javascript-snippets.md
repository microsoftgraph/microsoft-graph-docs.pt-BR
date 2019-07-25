---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 809173ab178f0fcd0697117fa989339300954f0d
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35719672"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getEmailActivityUserCounts(period='D7')')
    .version('beta')
    .get();

```