---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 82fc62d301155f5fe1b31b3ecf2e1b899dfbea0d
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48604139"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/contacts/{id}')
    .version('beta')
    .get();

```