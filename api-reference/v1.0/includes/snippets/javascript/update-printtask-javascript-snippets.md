---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1481772d13ab4468f15945e5b248fbd297706583dba596a2ed96ce4be33a4ff0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102747"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const printTask = {
  status: {
    state: 'completed',
    description: 'completed'
  }
};

await client.api('/print/taskDefinitions/{taskDefinitionId}/tasks/{taskId}')
    .update(printTask);

```