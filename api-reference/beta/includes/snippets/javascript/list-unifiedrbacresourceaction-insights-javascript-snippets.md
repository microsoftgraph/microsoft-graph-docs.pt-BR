---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d10741c862ed9dff414371fd2b5e4d6efdc064dd
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63337978"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let resourceActions = await client.api('/roleManagement/directory/resourceNamespaces/microsoft.insights/resourceActions')
    .version('beta')
    .get();

```