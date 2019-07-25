---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5e22b8dfec22959c7996e64356eae190434a7ea7
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35727547"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getMailboxUsageMailboxCounts(period='D7')')
    .version('beta')
    .get();

```