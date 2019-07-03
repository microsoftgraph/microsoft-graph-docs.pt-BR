---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8359efd783dbc4ae323b1ebf398e2f8959a2e3bd
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35518351"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/registeredDevices')
    .version('beta')
    .get();

```