---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: af9a996eb8d2abc2b825263d687fa1217d4668ef
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35477610"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const message = {
  isRead: "true",
};

let res = await client.api('/me/messages/{id}')
    .version('beta')
    .update({message : message});

```