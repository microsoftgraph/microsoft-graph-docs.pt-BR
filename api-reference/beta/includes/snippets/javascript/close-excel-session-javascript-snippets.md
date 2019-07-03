---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fefa9a5c9a41474db07d64004e237932aedffb2b
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35475603"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const closeSession = {

};

let res = await client.api('/me/drive/items/{id}/workbook/closeSession')
    .version('beta')
    .post(closeSession);

```