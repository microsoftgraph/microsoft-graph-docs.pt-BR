---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: db911671d1b74faf586141c5743c0cb909099609
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35498714"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/contacts/{id}')
    .version('beta')
    .delete();

```