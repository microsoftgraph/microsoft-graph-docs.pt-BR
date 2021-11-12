---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cd72a463b35fbe9e807c21ea09d7f472534d24bb0772fceb068c5b0cfaf3b35a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272101"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let tasks = await client.api('/me/planner/tasks')
    .version('beta')
    .get();

```