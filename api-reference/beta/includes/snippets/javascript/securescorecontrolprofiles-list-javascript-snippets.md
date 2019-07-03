---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e9f30271f1d4e997e66a0b20ce2b8dbe40238461
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35498201"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/security/secureScoreControlProfiles')
    .version('beta')
    .get();

```