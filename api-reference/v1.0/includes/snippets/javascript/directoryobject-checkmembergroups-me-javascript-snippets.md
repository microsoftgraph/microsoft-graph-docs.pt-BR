---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3ce2ed22dba1e61ffacee3069258cfa7d4d45c44
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/30/2021
ms.locfileid: "61224014"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const string = {
  groupIds: [
        'fee2c45b-915a-4a64b130f4eb9e75525e',
        '4fe90ae065a-478b9400e0a0e1cbd540'
  ]
};

await client.api('/me/checkMemberGroups')
    .version('beta')
    .post(string);

```