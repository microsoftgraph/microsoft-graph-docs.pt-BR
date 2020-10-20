---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 512bd57f245ec1a01fbaea3916138b645d865d73
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48619089"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/directoryRoles/{id}')
    .version('beta')
    .get();

```