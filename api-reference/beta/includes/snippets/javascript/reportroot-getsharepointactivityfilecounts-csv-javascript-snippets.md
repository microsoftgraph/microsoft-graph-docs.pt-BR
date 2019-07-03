---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 20ccd274ee71c51404db0c8bb475b7a3ee0da45d
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35518289"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getSharePointActivityFileCounts(period='D7')')
    .version('beta')
    .get();

```