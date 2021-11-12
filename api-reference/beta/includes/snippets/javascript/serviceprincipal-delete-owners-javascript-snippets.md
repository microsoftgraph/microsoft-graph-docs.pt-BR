---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a0f3257991aa8102ed56bcb916c186bf8a5fccaa48e8085f835f84c7a5e7669a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899048"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/servicePrincipals/{id}/owners/{id}/$ref')
    .delete();

```