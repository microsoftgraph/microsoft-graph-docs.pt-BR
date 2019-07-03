---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 310bbd17a1a2fb420ee7e2b0cfbb30bb7a7f5d97
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35499229"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/events/{id}/dismissReminder')
    .version('beta')
    .post();

```