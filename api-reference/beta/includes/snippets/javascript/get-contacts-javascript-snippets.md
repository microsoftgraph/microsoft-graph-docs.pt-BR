---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 49c0bea4151147a5d9bc07a4539214184e092f54
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35517735"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/contacts')
    .version('beta')
    .select('displayName,emailAddresses')
    .get();

```