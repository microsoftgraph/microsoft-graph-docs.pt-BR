---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 34873fe95c0657fb6f715084df0ce43cb77970a4
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35498707"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/threads/{id}')
    .version('beta')
    .delete();

```