---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8030deb7ef476408e4ddd08854b08e03c706285f8d1bac0f494dc87dff392fe5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100803"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let recentPlans = await client.api('/me/planner/recentPlans')
    .version('beta')
    .get();

```