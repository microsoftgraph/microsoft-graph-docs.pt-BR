---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 87d172bda4c1dd797860ed13647f0ed0ddf39c64
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48613899"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/contactFolders/{id}')
    .version('beta')
    .get();

```