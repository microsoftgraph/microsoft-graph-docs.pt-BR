---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 295ff960fc47fd9a6836fbaeb9a3ac5877cf48cd
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35508337"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/conversations/{id}')
    .delete();

```