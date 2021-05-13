---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f13d209bc789fb7d55bf2addcd89a55beed239d5
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2021
ms.locfileid: "52475162"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let roleAssignmentScheduleInstances = await client.api('/roleManagement/directory/roleAssignmentScheduleInstances')
    .version('beta')
    .get();

```