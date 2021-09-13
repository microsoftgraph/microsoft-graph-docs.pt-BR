---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4a8eb27c85095aa79fa89c8dbff276af017dccf885ba4390818c57c1748178f1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57326903"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let plannerTaskDetails = await client.api('/planner/tasks/{task-id}/details')
    .get();

```