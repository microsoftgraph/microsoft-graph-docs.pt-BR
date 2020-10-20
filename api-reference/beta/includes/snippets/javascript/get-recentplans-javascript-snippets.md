---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 18163aa07fa813d89e642b7a68b10b4c56fe46d0
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48609989"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/planner/recentPlans')
    .version('beta')
    .get();

```