---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bfdbca0a0c81b8b40fa01d5c0c205f4262e5f9de
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35476417"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users/delta')
    .version('beta')
    .get();

```