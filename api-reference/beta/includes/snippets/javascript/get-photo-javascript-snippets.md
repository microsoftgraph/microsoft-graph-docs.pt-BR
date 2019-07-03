---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 52acb6c01df80599566335969244cdf781782e6c
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35476600"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users/{id|userPrincipalName}/photo')
    .version('beta')
    .get();

```