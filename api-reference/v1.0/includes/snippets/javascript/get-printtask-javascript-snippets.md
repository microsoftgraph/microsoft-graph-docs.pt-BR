---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 07d170544eae75b519fb6da232524e7ab8fb61b51fdb10e397345350785d2a68
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329681"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let printTask = await client.api('/print/taskDefinitions/{taskDefinitionId}/tasks/{taskId}')
    .get();

```