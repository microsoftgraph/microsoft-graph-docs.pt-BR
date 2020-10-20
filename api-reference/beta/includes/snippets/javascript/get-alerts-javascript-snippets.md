---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fc3e8b106e3e2cdbee3005dce26af2d97a2df475
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48611612"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/security/alerts')
    .version('beta')
    .get();

```